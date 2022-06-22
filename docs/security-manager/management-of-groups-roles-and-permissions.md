# Management of Groups, Roles and Permissions

Setting up an PVSAS user account requires that administrators grant the exact permissions that 
allow the user to carry out their tasks within PVSAS, but no more. As mentioned, users get 
functionality access through their groups and data permissions either through groups or individually. 
In this section, you will find explanations of how to adapt individual user accounts, user groups, roles 
and permissions to design PVSAS accounts reflecting requirements from all users.

## Roles

Each naturally connected role in PVSAS should be defined as a role, where you can define the functions 
(tasks and operations) the user can carry out. Several roles are predefined that intended to distinguish 
between the responsibilities on each level of NPCs, NFs, and classifiers. To define a new role, click 
**Add Role** from the *User Roles* search form and complete the following details:

| **Field**         | **Format** | **Comments**                                                                                                                                                                                                                                                                                      |
| ----------------- | ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Role Code**     | text (30)  | Cannot be changed after creation; should not contain spaces; it is recommended to follow the CamelCaseSpelling like for already existing roles.                                                                                                                                                   |
| **Application**   | PVSAS      |                                                                                                                                                                                                                                                                                                   |
| **Level**         | drop-down  | see [User's Level](security-manager/user-accounts#users-level)                                                                                                                                                                                                                                    |
| **Description**   | text (200) | Descriptive label of the user roles; it is recommended to follow the examples of the predefined roles.                                                                                                                                                                                            |
| **Task Category** | text (8)   | Each operation and task is grouped. You can define which group(s) should be displayed only for this role by inserting the beginning of the group names. For a list of all existing task categories, see [Item Groups](security-manager/management-of-groups-roles-and-permissions.md#item-groups) |

After a role is created, all tasks (left column) and operations (right column) appear in the second part 
of the detail page. Click all tasks the role should allow and **Save** again. The slider in the middle reflects 
whether all, partial or no operations of the related tasked are enabled. In addition, the tab of *Role Groups* 
appears allowing you register the new role to one or more existing user groups.

## Item Groups

The item groups for a role define which functions appear in the lower part of the role detail page. 
As there are more than 200 different tasks and operations defined, it is recommended to restrict 
each role to one item group. The following item groups are defined, mostly representing one of 
the six PVSAS modules:
- ATHLETES – registration and classification of athletes
- CALENDAR – competitions and their officials, events and meetings
- C_CODES – sport and regional codes
- REPORTS – PVSAS report section
- SEC – Security/account manager
- SETTINGS – Application settings (basic codes, additional fields, news)
- TRACKER – access to the IPC Database Issue Tracker

## Role Functions

Each role the user has enables to complete certain tasks within PVSAS. The most common
tasks are the so-called CRUD tasks:
- Create: add a new item
- Read: read data on an item
- Update: edit an item
- Delete: remove an item from the system

These tasks are defined for nearly every section: e.g. athlete registration, athlete classification, 
license, competition, and so forth. Obviously, the tasks of creating, updating and deleting items are 
only useful if the user can read data from this section.

In addition, there are certain special tasks that enable only some parts of each section. For example, 
the *download sensitive class files* means the user is granted to download files uploaded under categories 
indicated as sensitive – it is designed for classifier to download these files while NPC/NFs can only upload 
but not open the documents in PVSAS.

## User Groups

The roles are gathered together into specific *User Groups*, which correspond broadly to the categories of 
user accounts described in [User Accounts](security-manager/user-accounts.md). When creating a new user account, 
you assign one or more groups with the specific roles and permissions. 

User groups can be added and removed from two screens: the user account details screen has a list of the user’s 
group, and the group details screen has a list of all users assigned to the group. This principle works generally 
for all types that are directly connected, as described in Figure 7.2; hence you cannot, for example, associate a 
user with a role or operation directly, but you can assign a user group to a data permission from the permission 
screen.

Some permissions, such as the federation permission, are badly suited for the assignment to a specific group; this 
would require a separate group for each country. Therefore, this permission is better set from the user page. 

As elsewhere in PVSAS, clicking on the code or name will bring up the details page for that item, and the details page 
also offers links to all users assigned to that item. 

Any of these methods will bring up a list of all available and assigned items of that particular type. Below is 
described how to add and remove user groups from a user whose account has already been created. The process for 
adding and removing roles and permissions works nearly analogously.

### How To: Add User Groups to an Account

1. Go to the *Security Manager* module and open the *User Accounts* search form.
2. Find the relevant user by entering required search criteria or scrolling through the result pages.
3. Click the user’s row to open the user’s details page; then click the *User Groups* tab to access the groups.
4. Find the desired group to add, either by scrolling through the result matrix for the available groups or by 
   using the search form in the *User Groups* tab (Figure 7.2).
5. Move the group between the available and assigned lists by dragging and dropping or selecting with the checkboxes 
   and clicking **Assign**.

To remove groups, you can select groups in the assigned groups list, and click **Remove**. The group will be moved to 
the available section and all relevant access derived from the associated roles is removed from the account.

### Data Permissions

PVSAS defines a single category of data permissions, that is for the national member federation of World ParaVolley. 
Each user must have access to at least one in that category; otherwise the user will not be able to access any athlete 
at all as each athlete is associated with one country.

One data permission is already pre-registered and allows full access to all data associated with all countries, coded 
with the %-character. This global permission cannot be deleted.

To register a new data permission, go to the search screen and click **Add Permission**. Select the permission category 
*National Federation* and enter the permission codes as follows:
- For a new national member of World ParaVolley, please check the NPC code as registered in regional application settings 
  (see [Members](application-settings/regional-data.md#members)). Then enter as permission code the found NPC code, 
  e.g. SUI for Switzerland.

Finalise the registration with a clear description of the data permission that could be just the country name and **Save**. 
Now the data permission is available for assignment to individual users or user groups.