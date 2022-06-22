# Website, Layout, and Functionalities

Some general information about the access to PVSAS as well as an overview of the structure and general functionalities and tools are outlined in this section.
# Access<!-- {docsify-ignore} -->

## PVSAS Website 
The World ParaVolley Sport Administration System is an online application accessible on the 
Internet by inserting the following URL in the browser of your choice

<p class="text-center">
  <a href="https://pvsas.worldparavolley.org" target="_blank">https://pvsas.worldparavolley.org</a>
</p>

<figure>
  <img src="_img/figures/2.1-pvsas-login-page.png" alt="PVSAS Login Page" class="screenshot">
  <figcaption>Figure 2.1 - PVSAS Login Page</figcaption>
</figure>

## Recommended Browsers 
It is recommended to use most modern and widely used browsers with recent updates 
installed to ensure stable functionality and security. PVSAS runs best under latest versions of [Firefox](https://www.mozilla.org/en-US/firefox/), [Google Chrome]([version](https://www.google.com/chrome/)) or [Microsoft Edge](https://www.microsoft.com/en-us/edge). Users of Internet Explorer (version 9 or higher) shall regularly update and inform about potential general security issues; and either download a 
stable version or look for alternatives. Additionally, JavaScript must be enabled for correct functionality of PVSAS.

> Please note that Internet Explorer has been retired by Microsoft and will be out of support as of June 15, 2022.

## User Accounts 
Currently, there are four main user groups defined. Besides the administrator account hold 
by the developer of PVSAS (the IPC) to review potential issues and change requests, 
accounts are granted to World ParaVolley, their classifiers, and their national members 
(NFs). World ParaVolley as supervisor of the ParaVolley classification processes can create 
accounts internally and for the NFs. By default, member federations and classifiers don’t 
have the rights to access the PVSAS user management. 

> [!DANGER]
> Please share your personal account details with any colleague only if you take on full responsibility for all actions performed through your PVSAS account.

### IF Accounts 
The IPC granted a few accounts to the IF to hand over full control on all further processes on 
launch in March 2018. The IF is able to create further accounts internally to share 
responsibilities and tasks.

### NF Accounts 
The IF distributes accounts to the recognized national member federations after launch. In 
case of an account issue, the IF must be contacted for support.

### Classifier Accounts 
In most cases, the IF management team automatically opens an account for the classifier 
with access to read out the most updated classification data as required for them to perform 
their duties at the competition. The classifier might gain rights to change data. Then it is 
highly recommended to carefully read the respective sections of the PVSAS manual about 
the update of classification values and files to ensure consistent and high data quality.

## Security and Passwords

PVSAS is a password-protected application. This protection requires high standard beginning with usage of strong passwords. Strength of a password is primarily defined by its length and its used character set. To find a compromise between security and user-friendliness, a password for PVSAS and all its related modules requires:

  &check; Minimum length of eight (8) characters

  &check; At least one (1) lower-case letter [a-z]

  &check; At least one (1) upper-case letter [A-Z]

  &check; At least one (1) numeric character [0-9]

  &check; At least one (1) non-alphanumeric character out of the set [!_%#?-@=$&+]

As it is recommended for all Internet applications, PVSAS automatically reminds the user to change his password when 360 days after last password change have passed.

> [!WARNING]
> Your account is automatically disabled after five sequential failed login attempts.

### Password Reset

The password reset tool can be used if you have forgotten your password, or if the account 
has been locked as described above. Instructions are given below.

#### How To: Change your password

1. After you have entered the application, go to **myAccount** at the upper right 
corner of PVSAS. This screen automatically opens after the 90 days period.


<figure>
<img src="_img/figures/2.2-sdms-password-editor.png" alt="Change Password" class="screenshot">
  <figcaption>Figure 2.2 - SDMS Password Editor</figcaption>
</figure>

2. Enter your current password in the first field. The new password is automatically 
controlled against the password requirements. Confirm your new password and 
submit.

#### How To: Reset password when you have forgotten it

1. Click on **I forgot my password** or use the menu bar **key reset**. 
2. Fill out the form by inserting your username and email address which had been 
registered with your account. 
3. After submission, you receive an automatically generated email with a password reset 
link. Check your spam folder if can’t find the message in your inbox. 
4. Follow the link. PVSAS opens and allows you to register a new password, respecting 
the password requirements. 
5. After confirmation and submission of your new password, navigate back to the login 
page.

<figure>
<img src="_img/figures/2.3-password-reset-email.png" alt="Auto-generated Email" class="screenshot">
  <figcaption>Figure 2.3 - Automatically generated email</figcaption>
</figure>

<figure>
<img src="_img/figures/2.4-password-reset.png" alt="SDMS Password Reset" class="screenshot">
  <figcaption>Figure 2.4 - SDMS Password Reset</figcaption>
</figure>

Please note that after submission of the password reset in step 2, you need to complete the 
remaining steps within 15 minutes. If this time has been passed without completion, you 
need to restart at step 1.

Passwords are stored encrypted. That means that no one, even not the PVSAS Administrator 
can read out your password. Same security standard is applied to other sensible information.

PVSAS logs you out after one hour of inactivity. This counter applies to each window or tab of 
your web browser independently from each other; but once your session is deleted in one of 
these tabs, your access in all of them is denied unless you re-login. This reduces the risk that 
a stranger with access to your terminal manipulates the data through your account without 
your knowledge. Especially in a public environment, it is highly recommended to click **Logout**
when you finished your work in PVSAS. 