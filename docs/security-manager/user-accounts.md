# Security Manager

The *Security Manager* module is where the database administrators (respective NPC and NF
staff) create, modify and access data related to user access of PVSAS. PVSAS needs to provide
access control to provide only relevant data for each user and to protect data privacy of all
athletes; this is implemented through Role-Based Access Control (RBAC). For a more thorough,
accurate and academic description of this system, please refer to introductory textbooks such
as *Role-Based Access Control, Second Edition* (Ferraiolo, Kuhn & Chandramouli, Artech Print, 2007).

The basic principle of RBAC is that a user has access permissions based on the job they
perform in the organisation. Each logically connected job is coded as a *user group*, with each
user able to be assigned to one or more groups. As several groups may share a similar role – e.g.
both NPC and NF officers should have access to the personal data about athletes in their sports
– the user groups function as an intermediate step linking to the *user roles*. The system checks
whether the users are a member of a role which has a certain access right before allowing their
access.

Continuing our example, consider the operation of viewing registered athletes, which is
accessible through several registration roles (administrative or read-only, or associated with a
specific NF), and full-access classification roles. Each user group can have several roles, with
permission being allocated on an OR basis, that is, it is only necessary for the user to be
member of one group with a particular functionality to access the pages enabled by that
functionality.

PVSAS also allows for a further layer of restriction permissions relating to sport and national
federation. Such permissions can be awarded directly to a user, for example if that user is an
officer of a specific NF, or to a user group. The sport and federation restrictions are
implemented on an AND basis with the roles as described above, so that the data must be both
relevant to one of the user’s roles and the user must have access to the sport and the country of
the data to be able to access it.

The sport and federation restrictions are set to none by default on user creation. For the user to
have an effective account, at least one sport and one federation must be set. NPC officers
should in most cases have access to information for all sports and federations (%-code).

<figure>
  <img src="_img/figures/7.1-pvsas-data-security.png" alt="PVSAS data security" class="screenshot">
  <figcaption>Figure 7.1 - PVSAS data security</figcaption>
</figure>

# User Accounts <!-- {docsify-ignore} -->

User accounts are created, deleted and modified in this section. The modification of user accounts 
also includes adding and deleting the user groups and permissions. This can, however, also be 
modified from the group screen or the permission screen. Currently, user accounts are available 
for the following broad of categories of users, described in more details in 
[User Accounts](layout-and-functionalities/access.md#user-accounts):

1. World ParaVolley Staff Members
2. NPC/NF Staff Members
3. World ParaVolley Classifiers

The following fields are available from the User Account Details page.

| **Field**    | **Format**                                                           | **Comments**   |
| ------------ | -------------------------------------------------------------------- | -------------- |
| **Username** | text (50 characters; case-sensitive letters, numbers, or underscore) | must be unique |

## Username and Password

The user must know his username and the associated password. When a new account is generated, 
the username must be unique, and the password obeys the password requirements as described in 
[Security and Passwords](layout-and-functionalities/access.md#security-and-passwords). 
The user details page also includes a *Password Requirements & Generator* tab, which generates 
a random password conforming to PVSAS standards by clicking **Generate**. Clicking **Focus** selects the 
generated password, which can then be copied and pasted to the user account page.

> [!DANGER]
> **Security Warning:** When creating a new account for a new staff member or client, 
> **DO NOT SEND THE PASSWORD** by email alongside the username. Either send the password 
> by a separate device (e.g. mobile phone) or instruct the user to use the *Account Activation* 
> from the PVSAS login page. During that process, the user requests to set up one’s own password 
> online after identification with username, email address, and a token valid for 15 minutes sent 
> to this email address.

## User’s Level

Each user account, user group, role and operation unambiguously belong to exactly one user level; 
these levels are *IF Admin*, *IF Staff*, *NPC/NF*, and *Classifier* in that order. Internally, these levels 
are just representing by a number to define the order. 

The value assigned to a specific user account finally determines which other user accounts, user groups, 
roles and permissions the user might have access to if (!) this person has access to the *Security Manager* at all.

Technically, it means: when a user is assigned to the user level X, he can read, add, delete and 
manipulate users, user groups, user roles and related operations of levels X and below. In an explicit case, 
level IF Admin can edit all as *IF Admin*, *IF Staff*, *NPC/NF*, and *Classifier* flagged items; level *IF Staff* can only 
edit *IF Staff*, *NPC/NF*, and *Classifier* so that superior organisations or accounts are protected. The IF admin can 
therefore create accounts for colleagues and IF members; an IF staff can handle accounts for colleagues as well, 
and for classifiers – but it prevents them from accessing/editing IF admin accounts.

## Logout Time and Failed Login Attempts

After the user has logged in, each page has a counter shown at the upper right corner (<img src="_img/inline/icon-login-timer.svg" alt="Login Timer" class="inline">)
next to the  logout icon that ticks down (shown in minutes). When this counter equals zero, a dialogue informs about 
the session’s expiration and requests to login again. The maximum value is 3600 s (= 60 minutes) but it is recommended 
to keep a value of 600 s (= 10 minutes) or lower. Users who do not properly log out might risk unauthorised access in 
an open network environment.

Each time the user failed to login with the correct username but with the wrong password, the *Failed Login Attempts* 
counter increases by one. As soon as this counter has a value of five (5) or higher, the user cannot login anymore 
unless the counter is reset manually clicking the <img src="_img/inline/icon-file-package.svg" alt="File Package" class="inline">
icon or the user requests a new password.

## Account and Password Expiration

To grant a temporary access to PVSAS, the *Account Expiry* has to be set to the last day PVSAS shall be accessible for 
this user. After that date the account is disabled. The user receives a respective message on login attempt with correct 
credentials. An account can also be immediately disabled by checking *Account Disabled*. 

Similar behaviour is applicable to the password. *Password Expiration* indicates when the user is requested to change the recent password. 
On the first login  attempt from that day onwards, the *Edit Password* screen automatically opens, and the user must enter follow the procedure; 
alternatively, he can only logout and do that step at a later point. Once the password is changed, the value here is automatically set to the 
date 360 days from today onwards. An account can also be requested to apply this behaviour immediately on next login of the user by checking 
*Password Change*.

## 2-Step Authentication

If this feature is enabled, the designated user not only needs his username and password, but also a **“token”**, in this case 
a six-digit number generated by an application the user must install (for free) on his mobile phone.

### First Set-Up
If the user has never logged in, yet – indicated by the fact that the *Authenticator Secret* is not generated – he will receive 
an instruction page and the secret for this account to set up his mobile phone after next login with correct credentials. 
Detailed instructions for Android devices, iPhone and similar, Windows Phone and BlackBerry devices are available on this page. 
Basically, the user needs to download one of the free available Authenticator apps, enter account and secret and save this information. 
Alternatively, to avoid typing errors, he can use the QR-code for direct import. Now the mobile app produces a six-digit number every 
30 seconds. It is important that the mobile’s internal time settings are accurate (more than one-minute difference to atomic time might 
cause login problems).

Once the mobile has been correctly configured and the user finds the code generating and changing each 30 second, he confirms his settings 
and clicks *Continue*.

This setting must be done only once.

### Login 

Each time the user now logins with correct username and password, he is asked for the number the mobile application currently shows. 
The user enters the number and clicks **Validate**. If correct, the user is redirected to his personal welcome page. Potential issues and 
first aid is listed in a small FAQ section underneath. In case, the user needs further support, direct contact to the responsible NF or NPC is recommended.

### Reset Configuration

In the case that the user lost the token (uninstalled the authenticator application on his mobile phone or similar), the responsible PVSAS security manager 
can open his account details and click the <img src="_img/inline/icon-authenticator.svg" alt="Authenticator Icon" class="inline"> icon. That removes the token 
registered so that the First-Setup page will show again after next login of the user.

### User Groups & Permissions

<figure>
  <img src="_img/figures/7.2-Assignment page of user groups.png" alt="Assignment page of user groups for a user" class="screenshot">
  <figcaption>Figure 7.2 - Assignment page of user groups for a user</figcaption>
</figure>

To display the user’s access rights, use the User Groups and User Permissions tabs. This shows all possible groups and permissions, 
and the user can be added to or removed from a group to change the account’s permissions. This is done by assigning from a list – 
the groups and/or permissions suitable to the user’s role are selected from the available result matrix and then moved to the assigned 
result matrix by clicking the assigning arrow. You can also drag and drop between the two lists to assign or remove objects and use the 
header fields to restrict your search if you want to access certain permission.

Please refer to the following sections for more information about the possible groups and permissions.
