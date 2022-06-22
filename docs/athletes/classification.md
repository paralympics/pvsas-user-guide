# Classification

More detailed information about classification, including signed forms, information about
historic classifications, details about the classification event, and so forth, are accessed from
this menu. This also allows for restriction of access, as Paralympic classification involves
sensitive medical information that should ideally be accessed by as few people as possible.

The section is organised by athlete, with a specifically designed search form for classification
relevant information. The athlete specific screen is then split into three tabs: The Classification
tab for viewing, modifying, adding, archiving and deleting classifications, the Profile tab where
medical information about current classifications may be added as text, and the Documentation
tab for upload of PDF scans of forms and sheets.

Only active athletes are listed in the classification search screen. To open the classification of a
retired or historic athlete, open the personal detail page and directly navigate to the athlete’s
classification with help of the <img src="_img/inline/icon-classification.svg" alt="Classification" class="inline"> icon.

## Classification Search Form

In addition to the fields displayed on the athlete search grid, the grid also shows the sport
and class of each athlete. The table below lists the possible search fields; none are
compulsory, by default the grid displays all athletes which the user can access. Only active
athletes are displayed in this search; if a user wishes to access information of retired
athletes, please use the registration search grid and navigate to the classification of the
retired athlete from the personal detail page via the <img src="_img/inline/icon-classification.svg" alt="Classification" class="inline"> icon.

| **Field**                                                     | **Format**         | **Comments**                                  |
| ------------------------------------------------------------- | ------------------ | --------------------------------------------- |
| **PVSAS ID**                                                  | integer boxes      |                                               |
| **Family name**                                               | text (30)          | searches for passport and preferred versions  |
| **Given name**                                                | text (30)          | searches for passport and preferred versions  |
| **Date of Birth**                                             | date (yyyy-mm-dd)  |                                               |
| **Gender**                                                    | drop down [gender] |                                               |
| **Member Federation**                                         | drop down [member] |                                               |
| **Class**                                                     | text (50)          | text search (e.g. F3 would find F34, F35 etc) |
| **Class Status**                                              | dropdown [N/R/C]   |                                               |
| **Classification Date**</span><span class="asterisk">*</span> | date (yyyy-mm-dd)  | exact date of classification                  |
| **Year of Review**</span><span class="asterisk">*</span>      | year (yyyy)        | year of scheduled review                      |
| **Classifier**</span><span class="asterisk">*</span>          | text (50)          | searches for all classifier fields (1-3)      |

<p class="footnote">
    <small><span class="asterisk">*</span>Data for these fields only appear when the Grouping parameter is set to by class.</small>
</p>

By default, each class of each athlete is displayed in a row. This behaviour can be changed
by setting the advanced search parameter *Grouping* to *by athlete*. Then each row represents
one athlete with all current classes if he has two or more. However, selecting an athlete
opens the classification detail page including all classification the athlete is registered in.

## Classification Details

<figure>
    <img src="_img/figures/4.3-classification-details.png" alt="Classification Details" class="screenshot" >
    <figcaption>Figure 4.3 - Classification Details</figcaption>
</figure>

When opening an athlete’s classification details page (Figure 4.3), each classification
instance has its own row in its respective section (*Current* or *Historical*). Any current
classification not with *New* status should be accompanied by documentation and
confirmation from classifiers. If the athlete’s class changes, this should be documented by
adding a new classification row and moving the outdated one to *Historical* status.

In the table below, those fields are listed in the form that can be accessed from the New
*Classification form* (Figure 4.4) when defining a new classification for an athlete.

| **Field**                       | **Format**                      | **Comments**                                                                                                 |
| ------------------------------- | ------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| **Sport**                       |                                 | Defaults to ParaVolley                                                                                       |
| **Class**                       | text (50)                       | List of ParaVolley classes and pseudo-classes                                                                |
| **Class Status**                | *Confirmed*, *Review*, or *New* | Applied to all selected classes.                                                                             |
| **Year of Review**              | year (yyyy)                     | Year of scheduled review.                                                                                    |
| **Classification Date**         | date (yyyy-mm-dd)               | **Tip:** the small **‘+’** opens a drop-down to indicate the order of classification panels of the same day. |
| **Classifier 1-3**              | text (50)                       | Name of acronyms of the responsible classifier(s).                                                           |
| **Reason of Re-Classification** | drop-down [BAC, MRR, PuEC, WPV] | Applicable reasons</span><span class="asterisk">*</span>                                                     |
| **Limitation**                  | drop-down box [class group]     | only appears in the classification table                                                                     |

<p class="footnote">
    <small>
    <span class="asterisk">*</span> <b>BAC</b> (Board of Appeal of Classification) | <b>MRR</b> (Medical Review Request) | <b>PuEC</b> (Protest under Exceptional Circumstances) | <b>WPV</b> (Appeal through WPV)</small>
</p>

Following additional fields appear only in the classification table, not in the registration form for new classifications:

| **Field**                                                    | **Format**               | **Comments**                                                                                                                                                              |
| ------------------------------------------------------------ | ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Date of Classification order (+)**                         | integer                  | Click the small ‘+’ next to the classification date field. A little drop down allows to indicate the order of classification panels of the same day with the numbers 1-3. |
| **Limitation (group)**</span><span class="asterisk">*</span> | drop-down [class groups] | Limits the class to the selected class group (see [Sport Codes](application-settings/sport-codes.md))                                                                     |

<p class="footnote">
    <small>
    <span class="asterisk">*</span>Each standard class is associated with one of the ParaVolley disciplines (standing or sitting), however, pseudo-classes (like NE, CNC) must be specified. 
    <br />
    If an athlete only has ‘NE’ as class, the system cannot identify which discipline he belongs to. 
    <br />
    This assignment is necessary for the correct analysis in the classification reports. 
    <br />
    If the class group is not specified for a pseudo-class, PVSAS will consider the athlete as not eligible across all disciplines.
</small>
</p>

When the outcome of a recent classification panel shall be registered, the old information
currently appearing under *Current Classification* should be kept in the history. Therefore, the
section of current classification has no delete button. Users may archive current
classifications by selecting their row(s) and clicking the **Move to History** button; the
classification then ceases to take effect on any future results, but the record remains in the
database, can be viewed from the classification analysis, and affects past results. If a
classification is added in genuine error, it may be deleted from the historical section by
selecting its row and then clicking the **Delete** button.

### How To: Report a Change in Classification

<figure>
    <img src="_img/figures/4.4-adding-new-classes.png" alt="Adding new classes" class="screenshot" >
    <figcaption>Figure 4.4 - Adding new classes</figcaption>
</figure>

1. Search for the athlete from the Classification search form using any criteria available. 
   Click on the row of the athlete to bring up the *Classification Details* screen.

2. Click **New Classification** to bring up the associated entry form.

3. Using the table of fields in this section as reference, enter the details of the athlete’s 
   new classification. Sport, one class, the new status and the date of classification are 
   required fields; sport, class and status may not be changed once added.

4. Add any special restrictions in the *Limitation* column.
   
5. Select the previous class(es) by clicking associated tick box(es) in front of the row(s) 
   and click **Move to History**. All selected classes are moved down to historical classification 
   so that only the most recent classification shall appear in the upper table.

6. If you have any documents to upload, go to the *Files* tab of the relevant sport.
   
7. Click the <img src="_img/inline/icon-browse.svg" alt="Browse" class="inline"> or the 
   <img src="_img/inline/icon-replace.svg" alt="Replace File" class="inline">icon (if a file is already attached) 
   in the row of the relevant document, e.g. classification sheet, medical form, protest sheet.

8. Select the document from your local hard drive or network and click **Open**. If successful, the file has 
   been immediately uploaded and any previously stored file under this category is automatically moved to the file archive underneath.

## Classification Profile

The *Profile* tab displays information about the athlete’s medical details. This tab is organised
in sections by sport, with each section having text fields, drop-down menus or checkboxes
specific to the classification report compiled by classifiers in each sport. When data are
changed and saved, previous values are overwritten.

The fields are pre-defined but can be changed by the IPC. This allows a high degree of
flexibility to store important data separately from the generics (class and status) and the
PDFs. Information from these fields are exportable in the classification master lists reports
(see [Classification Master List](reports/classification-master-list.md)).

## Documentation

The Documentation tab allows for uploading and accessing sheets and forms relating to
classification issues. Each athlete has one files tab per sport they are registered in.

<figure>
    <img src="_img/figures/4.5-classification-documents.png" alt="Classification Documents" class="screenshot" >
    <figcaption>Figure 4.5 - Classification Documents</figcaption>
</figure>

The upload process is described in the [*How-To: Report a Change in Classification*](athletes/classification.md#classification-details#how-to-report-a-change-in-classification). 
The files are stored in one of two sections, recent or historical. The section about recent classification 
files is separated into several containers. These containers, like the classification profile fields, 
can be changed by the IPC.

In the section about the additional fields, there are two sets of file categories. The first one,
called *Classification Files (basic)*, allow the flexible up- (<img src="_img/inline/icon-replace.svg" alt="Replace File" class="inline">) 
and download (<img src="_img/inline/icon-download-document.svg" alt="Download Document" class="inline">) 
by any user who is granted to access this section. In Figure 4.5, these are the classification, the protest, 
and the medical review sheets. The second one is called *Classification Files (sensitive)* and is 
indicated in the classification file section with an asterisk (*). Users with the basic rights to 
upload files can perform the browse and upload function but are not able to read the file thereafter 
(<img src="_img/inline/icon-confidential-file.svg" alt="Confidential File" class="inline">). 
For access to files uploaded to these sensitive categories, the user must fulfil several conditions 
that are described further down.

### How To: Protect and access a sensitive classification file, e.g. a medical diagnosis.

Some files which must be accessed by classifiers contain very sensitive data about the
athlete’s conditions. Due to data protection laws these files must not be accessible all the
time and only by a controlled group of persons.

These files should be uploaded to a file category that is defined as *sensitive*. Sensitive
categories are marked with an asterisk (*) in the documentation section. Basic users can
upload but not download (<img src="_img/inline/icon-confidential-file.svg" alt="Confidential File" class="inline">) 
a file associated with such a category.

Classifiers require reading the file for the upcoming classification panel. To grant one or more
classifiers to access the sensitive files, following steps must be undertaken:

1. Under *Calendar > Competitions*, the upcoming classification panel must be registered with an end date later than today (see [Sport-specific management](calendar/competitions.md#sport-specific-management)).
2. The athlete must be registered as participant (see [Assigning Athletes and Classifiers](calendar/competitions.md#assigning-athletes-and-classifiers)).
3. The classifier must be registered as such under *Calendar > Officials* **and** his username of his PVSAS account must be included in his classifier profile (see [User Accounts](layout-and-functionalities/access.md#user-accounts)).
4. The classifier must be registered as classifier of this panel (see [Assigning Athletes and Classifiers](calendar/competitions.md#assigning-athletes-and-classifiers)).

With help of these settings, the system checks that the user is a registered classifier for the 
upcoming panel so that he requires and gets access to all documents uploaded to PVSAS of 
those athletes who undergo classification at the same panel.

As soon as the classification panel has passed – this means, the end date of the classification panel 
is in the past – the respective classifiers won’t be able to access the files any more. The files are 
again fully protected unless athletes and classifiers are assigned to a new upcoming event.

When immediate action is required for a classifier or athlete, the respective person just needs to be unassigned from the panel.