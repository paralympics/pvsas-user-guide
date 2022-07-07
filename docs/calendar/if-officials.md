# IF Officials

Officials of World ParaVolley can be classifiers, technical officials or judges. 
Classifiers are assigned to competition sports (see [Sport-specific management](calendar/competitions.md#sport-specific-management)). 
Similar to the athletes, each classifier obtains a unique ID holding a very few 
personal details and a list of his/her roles active and inactive roles.

| **Field**                                       | **Format**         | **Searchable** | **Comments**                                                                                                   |
| ----------------------------------------------- | ------------------ | -------------- | -------------------------------------------------------------------------------------------------------------- |
| <span class="table-header">Personal Data</span> |                    |                |                                                                                                                |
| **Official ID**                                 | number             | Yes            | automatically assigned on participant creation                                                                 |
| **Family Name**                                 | text (50)          | Yes            |                                                                                                                |
| **Given Name**                                  | text (50)          | Yes            |                                                                                                                |
| **Gender**                                      | radio buttons      | No             | male or female                                                                                                 |
| **Date of Birth**                               | date               | No             | male or female                                                                                                 |
| **Country of Residence**                        | drop-down[country] | No             | male or female                                                                                                 |
| **Email**                                       | email(50)          | Yes            | correct email address of the classifier; required for availability request process                             |
| **Application Username**                        | text(50)           | No             | see comments below                                                                                             |
| **Mobile Phone**                                | text(20)           | No             |                                                                                                                |
| **Landline Phone**                              | text(20)           | No             |                                                                                                                |
| **Photo**                                       | image              | No             | optional, same requirements as for athletes                                                                    |
| **Comments**                                    | text               | No             |                                                                                                                |
| <span class="table-header">Roles</span>         |                    |                |                                                                                                                |
| **Sport**                                       | ParaVolley         | No             |                                                                                                                |
| **Category**                                    | drop-down          | No             | Classifier, Technical Official, Referee, Judge, Linesman (depending on sport)                                  |
| **Impairment**                                  | PI                 | No             | default value for classifiers                                                                                  |
| **Activity**                                    | active or inactive | No             | Set to inactive to avoid the classifier as available in assignment pages or for the attendance request process |
| <span class="table-header">Languages</span>     |                    |                |                                                                                                                |
| **Name**                                        | text (50)          | No             | Name of language the official is skilled in (English and local)                                                |
| **Skill**                                       | drop-down          | No             | Skill level: native, fluent, good, basic                                                                       |

Each official must retain at least one role and one language. During first 
registration, the first role is registered and automatically activated. 
In addition, the native language is registered. 

After submission of first registration, further roles and languages can be 
added by clicking the **+ Add New Role** button under the corresponding table. 
Once a role or language is registered, it cannot be edited (except the activity 
status for roles and the skill level for spoken languages) but deleted 
(<img src="_img/inline/icon-delete.svg" alt="Delete Role" class="inline svg-small">) 
and newly registered if necessary.

## Classifier Registration vs Classifier User Account

Classifiers must be registered in this section here separately as (1) not each 
classifier directly has an account to PVSAS, and (2) when the classifier user 
account is removed, information stored about or from the classifier still should 
remain in the system.

The picture below visualises the various entities that must relate to each other 
to grant a classifier access to sensitive files of an athlete.

<figure>
    <img src="_img/figures/5.3-role-of-classifier-registration.png" alt="Role of classifier registration to access sensitive files" class="screenshot center" >
    <figcaption>Figure 5.3 - Role of classifier registration to access sensitive files</figcaption>
</figure>

Both, the classifier and the athlete must be assigned to the same classification 
event in the PVSAS calendar whose end date must be in the future. To allow a 
classifier user to access now the athlete’s classification marked as *sensitive*, 
the classifier registered here must be linked to the user account. This link is 
established by entering the username under *Application Username*. Then PVSAS 
knows that the user is a proper classifier (the user group is not involved in 
this identification) and runs the control algorithm to grant or lock access to 
the sensitive files. Further information can be found in 
[Classification Details](athletes/classification.md#classification-details) and 
[Assigning Athletes and Classifiers](calendar/competitions.md#assigning-athletes-and-classifiers).