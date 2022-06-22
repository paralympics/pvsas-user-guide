This section describes the menu items related to the administration of events and attendance
of classifiers and technical officials to competitions or classification panels. The calendar allows
for panels in all sports to be entered, including athletes and classifiers to participate that also
influences the access rights of PVSAS classifier users to open sensitive files of these athletes
(see [Documentation](athletes/classification.md#documentation)).

# Competitions 

From this screen, competitions or classification panels not associated with a competition can be
created and deleted. Each event has one or more sports associated with it that participants
(athletes and classifiers) can be assigned to.

An event is uniquely identified by its 6-character code, which is generated during the
registration in PVSAS. This code has the format **SSCCDD**, where the digits signify
-  **SS:** the sport code for the event
-  **CC:** arbitrary combination of letters and numerals that may reflect the event level, name, or city.
-  **DD:** last two digits of the year of the event, derived from event start date. The first and the last 
    parts of the code are automatically generated based on the

The first and the last parts of the code are automatically generated based on the select sport 
and season of the event. The middle part can be either specifically defined. If not defined, the 
system will automatically find out a unique but random combination.

A new competition or classification event is created by clicking **Add Event** from the 
competitions & events search grid.

The following data is available to enter from the details screen.

| **Field**                                           | **Format**              | **Searchable**          | **Comments**                                                                                                                     |
| --------------------------------------------------- | ----------------------- | ----------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| <span class="table-header">Basic Information</span> |                         |                         |                                                                                                                                  |
| **Sport**                                           | drop-down box [sport]   | Yes                     | Defaults to ParaVolley                                                                                                           |
| **User-defined code**                               | text (2)                | Yes, part of event code | Only available on new registration. Defines the middle two digits of the event code. Keep blank to let PVSAS find a random code. |
| **Competition Code**                                | text (6) A-Z or numbers | Yes, also as substring  | Auto-generated based on sport, user-defined code and competition start date.                                                     |
| **Season**                                          | drop-down [value list]  | Yes                     | see [Seasons](application-settings/configuration.md#seasons)                                                                     |


PVSAS shares the competition calendar with the IPC Sport Data Management System. 
However, ParaVolley specific competitions can only be accessed in PVSAS while IPC specific 
competitions only in IPC SDMS. The advantage is that multi-sport events like the Paralympic
Games can be accessed by both, and the responsible federation may edit the sport-specific data.

## Sport-specific management

<figure>
    <img src="_img/figures/5.1-adding-more-sports.png" alt="Adding more sports" class="screenshot" >
    <figcaption>Adding more sports</figcaption>
</figure>

Once the event is saved, two more tabs appear, labelled *Sports* and the name of the sport initially 
selected during first registration. New sports cannot be registered. Multi-sport competitions like 
the Paralympic Games are registered by the IPC. The list of sports to review is not filtered by the 
user’s sport restriction. Each sport detail tab has the following information. All fields are optional 
but might provide sport-specific details, in particular in case of a competition.

| **Field**                                       | **Format**               | **Comments**                                                                                       |
| ----------------------------------------------- | ------------------------ | -------------------------------------------------------------------------------------------------- |
| <span class="table-header">Event Details</span> |                          |                                                                                                    |
| **Competition Code**                            | text field, unmodifiable | These fields are included for cross reference and must be modified at the competition details tab. |

Additionally, sport-specific contact details can be registered. The fields are identical to those 
from the general detail page of the event without organiser and website reference.

## Assigning Athletes and Classifiers

At the bottom of the sport-specific event page, there are two buttons labelled *Athletes* and *Classifiers*. 
Each of them opens an assignment page to register athletes and classifiers, respectively, in this particular 
sport for the current event.

<figure>
    <img src="_img/figures/5.2-athletes-assignment-to-an-event.png" alt="Athletes assignment to an event" class="screenshot" >
    <figcaption>Athletes assignment to an event</figcaption>
</figure>

On the left side, all available athletes/classifiers as registered in PVSAS are listed. The right table 
shows all registered (assigned) persons to this competition sport. Registration or removal is handled 
by either moving a row by drag&drop from one table to the other one, or by selecting several persons 
and clicking either the button **Assign** or **Remove**.

Both assignment pages additionally offer the **Mass Assignment**. It opens a dialogue box to enter or 
copy&paste from an Excel table a list of athlete or classifier IDs. The separator between each ID can 
be any character like line breaks, the comma, semi-colon etc. When the **Assign** button in the dialogue 
is clicked, PVSAS tries to find all athletes/classifiers with the entered IDs and assign them to the event 
in the given sport. Invalid numbers will be ignored, and the user will be informed about that to review 
potential typing errors or registration information of the associated person.

The user might be reminded the criteria to grant a classifier access to an athlete’s medical documents 
outlined in [Documentation](athletes/classification.md#documentation); only if the classifier and the 
athlete are assigned to the same event, the classifier registered as PVSAS user is able to open files 
categorised as *sensitive* for this particular athlete. As soon as the event has passed, the files are 
automatically locked unless classifier and athlete are assigned to a new event in future. It is not 
necessary to manually undo the assignment for past events.

