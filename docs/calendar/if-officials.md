# IF Officials

Officials of World ParaVolley can be classifiers, technical officials or judges. 
Classifiers are assigned to competition sports (see [Sport-specific management](calendar/competitions.md#sport-specific-management)). 
Similar to the athletes, each classifier obtains a unique ID holding a very few 
personal details and a list of his/her roles active and inactive roles.

| **Field**                                       | **Format** | **Searchable** | **Comments**                                   |
| ----------------------------------------------- | ---------- | -------------- | ---------------------------------------------- |
| <span class="table-header">Personal Data</span> |            |                |                                                |
| **Official ID**                                 | number     | Yes            | automatically assigned on participant creation |

Each official must retain at least one role and one language. During first 
registration, the first role is registered and automatically activated. 
In addition, the native language is registered. 

After submission of first registration, further roles and languages can be 
added by clicking the 
<img src="_img/inline/icon-add.svg" alt="Add Official Role" class="inline"> 
icon under the corresponding table. Once a role or language is registered, 
it cannot be edited (except the activity status for roles and the skill 
level for spoken languages) but deleted (<img src="_img/inline/icon-delete.svg" alt="Delete Role" class="inline">) 
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
    <figcaption>Figure 5.3: Role of classifier registration to access sensitive files</figcaption>
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