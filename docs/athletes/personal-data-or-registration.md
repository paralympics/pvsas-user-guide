# Athletes

This chapter described the core section of PVSAS, where users can read and modify personal 
data relating to ParaVolley athletes across all national federations and manage their 
classification individually.

Once an athlete has been selected from the registration, the classification, or the nationality 
screen, each other athlete’s page can be directly opened clicking the corresponding icon at the 
upper right corner next to athlete’s ID and name.

<img src="_img/inline/personal-detail-page.png" alt="Personal Detail" class="center inline"> Opens the personal detail page

<img src="_img/inline/classification-page.png" alt="Classification" class="center inline"> Opens the classification page

<img src="_img/inline/nationality-page.png" alt="Nationality" class="center inline"> Opens the nationality page

## Personal Data / Registration <!-- {docsify-ignore} -->

Each athlete must be registered first before any further classification information and files can 
be associated. From this menu, the user has access to all registered athletes he can access 
based on his access federation and sport related access rights.

## Details

Users must navigate the **Athlete Registration** search screen before they can modify any 
participant details. By clicking on a row in the grid or on the *Add Athlete* button, users reach 
the details tab with fields described in the following table. Certain fields are mandatory 
to fill out on creation or update of an athlete.

| **Field**                                                                                           | **Format**                                               | **Searchable** | **Comments**                                                                                                                                                                                       |
| --------------------------------------------------------------------------------------------------- | -------------------------------------------------------- | -------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span class="table-header">Basic Information</span>                                                 |                                                          |                |                                                                                                                                                                                                    |
| **Athlete ID**                                                                                      | number                                                   | Yes            | automatically assigned on participant creation                                                                                                                                                     |
| **Career Status**                                                                                   | *Active*, *Historical* or *Retired*                      | Yes            | always set to active on creation, must be changed at *Career Status* tab                                                                                                                           |
| <span class="table-header">Personal Data</span>                                                     |                                                          |                |                                                                                                                                                                                                    |
| **Member Federation**                                                                               | drop down [member]                                       | Yes            | obligatory, loaded from member basic table; the drop-down is limited to the list of World ParaVolley (see [Application Settings](application-settings/regional-data.md#international-federations)) |
| **no Family Name**                                                                                  | checkbox                                                 | No             | in some cultures, only the given name is used in the passport. This box may be ticked to allow entries of such athletes; if not ticked, then both family and given names are obligatory fields     |
| **Family Name (passport)**                                                                          | text (30)                                                | Yes            | family name exactly as written in the passport (except for non-English characters).                                                                                                                |
| **Given Name (passport)**                                                                           | text (30)                                                | Yes            | given name exactly as written in the passport. This is culturally dependent, but usually the name that appears second in the passport                                                              |
| **Family name (preferred)**                                                                         | text (30)                                                | Yes            | the version of the family name that will be used in all PVSAS output. May be left blank on entry, will then be identical to passport name                                                          |
| **Given name (preferred)**                                                                          | text (30)                                                | Yes            | as above but with given name                                                                                                                                                                       |
| **Gender**                                                                                          | radio buttons                                            | Yes            | obligatory                                                                                                                                                                                         |
| **Date of Birth**                                                                                   | date (yyyy-mm-dd)                                        | No             |                                                                                                                                                                                                    |
| **Photo**                                                                                           | picture file                                             | No             | set by system or by the user under nationality validation, see [File Attachments](layout-and-functionalities/file-attachments.md)                                                                  |
| <span class="table-header">Nationality Information</span>                                           |                                                          |                |                                                                                                                                                                                                    |
| **Nationality**                                                                                     | drop down [country demonym]                              | Yes            |                                                                                                                                                                                                    |
| **Nationality Status**                                                                              | read-only                                                |                | obligatory, should be the same as NPC unless there can be made an exception for the athlete under the IPC Nationality Policy (see [Nationality Validation](athletes/nationality-validation.md))    |
| **Validation Document**                                                                             | drop down [*Passport*, *ID Card* or *Birth Certificate*] | No             | type of referenced document                                                                                                                                                                        |
| **Date of Expiration**                                                                              | date (yyyy-mm-dd)                                        | No             | date this document stops being valid, as determined by the issuing authority. A checkbox may be ticked if the referenced document never expires                                                    |
| **Passport/ID Card No**                                                                             | text (30)                                                | Yes            | ID number of the referenced document                                                                                                                                                               |
| **Copy of Passport/ID Card**                                                                        | PDF file                                                 | No             | to upload a scan of the referenced document from user’s hard drive or local network. Once uploaded, the document can be downloaded or replaced.                                                    |
| **Previous Member Representation**                                                                  | drop down [NPCs]                                         | No             | only applicable for athletes who have previously competed for other NPCs                                                                                                                           |
| **Confirmation Document**                                                                           | PDF file                                                 | No             | uploaded by WPV after a nationality issue has been reviewed and confirmed                                                                                                                          |
| <span class="table-header">Sport and Sport Class Registration</span><span class="asterisk">*</span> |                                                          |                |                                                                                                                                                                                                    |
| **Sport Class**                                                                                     | drop down [class]                                        | No             | populated upon selection of a sport                                                                                                                                                                |
| <span class="table-header">Comments</span>                                                          |                                                          |                |                                                                                                                                                                                                    |
| **Member Comments**                                                                                 | text                                                     | No             | further free text information that can be provided by the member federation                                                                                                                        |
| **World ParaVolley Comments**                                                                       | text                                                     | No             | further free text information that can be provided by the IF; the member federation can only read but not change its content.                                                                      |

<p class="footnote">
    <small><span class="asterisk">*</span>Only available and displayed at registration of a new athlete. Any further modification must be done at the **Sports & Classes** tab or through the classification section of PVSAS.</small>
</p>

The *searchable* column indicates whether this field is offered as a criterion on the search form. 
The *family name* and *given name* fields of the search form will match in either the passport or 
preferred name fields, but only display the preferred name, which may sometimes lead to unexpected search results. 

<img src="_img/inline/delete-button.png" alt="Delete Button" class="center inline-button">

> [!DANGER]
> **Caution:** The **‘delete’** button is accessible from the participant detail menu. An athlete may be 
> completely deleted from the system once the user confirms a security question. **On deletion, all related classification data and files are irrevocably removed from the system.** 
> In case, you want to remove just a duplicate, it is highly recommended to use the merging tool in the duplicate control section, see [Duplicate Control](athletes/duplicate-control.md). 
> If the athlete is not active in this sport any more, the status shall be changed to **‘Retired’**.

### How To: Register a new Athlete 

<img src="_img/inline/new-button.png" alt="New Athlete/Guide Button" class="center inline-button">

1. Obtain a blank athlete detail form (see Figure 4.1) by clicking the **Add Athlete** button (from the search form) 
   or the **New** button (from the details page). 
2. Referring to the athlete details table, complete all fields to the best of your knowledge. Yellow fields are mandatory. 
   Cross-check spelling and information with the uploaded documents, the athlete family and given name according to their passport. 
3. Select the class the athlete is either already classified in on national level, or the class the athlete is likely to be. 
   This is required to give the responsible federation and their classifiers access to this athlete for classification input. 
   Class status will be automatically set to *New*. 
4. Click **Save** to create an Athlete ID for the athlete. 

<figure>
    <img src="_img/figures/4.1-athlete-registration-create.png" alt="A blank athlete registration form including file upload information" class="screenshot" >
    <figcaption>Figure 4.1 - A blank athlete registration form including file upload information</figcaption>
</figure>

When saving an athlete for the first time, the system automatically searches for potential 
duplicates based on various combinations of name, date of birth, gender, and passport 
information. If one or more potential duplicates are found, a dialog box opens listing them. It 
is then possible to either proceed registering the new athlete under a new ID, open one of the 
existing profiles or cancel the registration completely for further amendments. 

Photo and other documentation can be uploaded during or after first registration anytime. 
Click the <img src="_img/inline/icon-upload-image.svg" alt="Upload Image" class="inline"> 
icon to select the athlete’s photo from your local hard drive or network. The requirements for 
photos are described in chapter 2.5. For quick reference, the photo should be in passport size 
format, around 7:10 in aspect ratio, and saved as a JPG file smaller than 250 kB. Click the 
<img src="_img/inline/icon-browse.svg" alt="Browse" class="inline"> icon to select the athlete’s 
passport copy or IPC nationality letter in PDF format from your local hard drive.

After an athlete has been registered, there may be reason to change the details, for example 
because of errors or omissions in the data entry process, name changes due to change in 
marital status, etc.

### How To: Change Athlete Details

1. Search for the athlete in question from the **Athlete Registration** search form and click the row 
   in the search grid corresponding to the athlete to enter the athlete details’ page. 
2. The data stored about the athlete will appear in the form. Edit the incorrect or missing details and click **Save**. 
3. If you change passport name and/or the member federation of the athlete, a dialogue box (see Figure 4.2) appears 
   to ask you to confirm the reason for the name change. Choose one of the three supplied reasons (error, marriage or nationality change) 
   and, if applicable, enter the date from which the change should be effective. 
4. If you change the name of the athlete, please bear in mind that changes only apply to the field you enter, i.e., a change of passport 
   name will not change the preferred name, which is how the athlete will be named in publications. Hence, in case of a name change, please 
   change both fields unless there is a specific reason not to; e.g. the athlete wishes to be known under the old name but the passport issuing 
   body will only recognise the new name.

<figure>
    <img src="_img/figures/4.2-name-change-dialogue-box.png" alt="Name change dialogue box" class="screenshot center" >
    <figcaption>Figure 4.2 - Name change dialogue box</figcaption>
</figure>

## Career & Name Changes

The content of this tab is separated into three parts.

The upper part allows the user changing the career status of the athlete. To change the 
status, enter a reason for the career status change, select the new status and **Save**. Retired 
and historic athletes can be or are automatically excluded from search grids and reports. 
Historic athletes can be excluded from user’s view by removing the operation *find historic athletes* 
from the user’s roles (see [Role Functions](security-manager/management-of-groups-roles-and-permissions.md#role-functions)).

The second part reflects all the career status changes including the provided reason and 
timestamps.

The lower part reflects the changes of the athlete’s name and NF association. Each 
(passport) name change is registered in the database to ensure that the identification of the 
individual for an athlete ID never changes. The table here only shows the changes due to 
marriage (M) or nationality (N) changes, but all error (E) related changes are still registered in 
the backend and can be requested by the IPC SDMS administrator. 

## Biography

This tab is designed for adding, modifying and removing data about the athlete’s life to date. 
This is particularly designed for media and fan interaction with the athletes, allowing them to 
get to know the athletes’ personality beyond a statement of their results. 

The biography tab is designed to be easily modifiable in case fields need to be added or removed 
and should hopefully be self-explanatory. Fields are labelled in the left-hand column and a more 
detailed explanation, if necessary, is given in the right-hand column.

## Data Sheet

Core information about an athlete is summarised in the data sheet report, including personal
information, the photo, registration statuses and the classification history.
This sheet appears as PDF inside the tab. If your browser does not support the PDF plugin,
you can click the link to generate and download the PDF to your local storage.