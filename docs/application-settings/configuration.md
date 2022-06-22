# Application Settings

This section describes all screens of the first PVSAS module **Application Settings**. Obviously, 
all basic or core entities can be managed or at least viewed here, like sports, events, 
organisations, or seasons as well as some more technical settings.

# Configuration <!-- {docsify-ignore} -->

## Seasons

Competition calendars either use the summer sport seasons (1 January to 31 December) or 
winter sport seasons (1 July to 30 June of the subsequent calendar year). Consequently, 
each competition must be assigned to a specific season. By default, it is the season the 
competition takes place in, but exceptions can be applied if, for example, a licensing 
programme is in place.

For World ParaVolley, the season between 2017 and 2020 are pre-configured. Additionally, 
with ParaVolley considered as summer sport, seasons are automatically considered as 
summer seasons.

| **Field**      | **Format**        | **Comments**                                                                                                            |
| :------------- | :---------------- | :---------------------------------------------------------------------------------------------------------------------- |
| **Code**       | text (3)          | Please follow the standard format Snn with nn as the two-digit year of the start date (e.g. S24 for summer season 2024) |
| **Name**       | text (50)         | Unique season name; should follow the pattern “Summer Season yyyy” with yyyy as full year qualifier.                    |
| **Start Date** | date [yyyy-mm-dd] | First day of season                                                                                                     |
| **End Date**   | date [yyyy-mm-dd] | Last day of season                                                                                                      |
| **Status**     | drop down         | **only used if a licensing programme is enabled**                                                                       |
| **Comments**   | text (200)        |                                                                                                                         |

The open date fields allow a flexible definition of seasons even outside the standard pattern.

## Application News

On the left-hand side of the PVSAS login page, short news can be flexibly published, e.g. 
about the update the application, introduction of new regulations, links to important 
documents and more. By default, World ParaVolley as owner of PVSAS can add, remove and 
change articles for this news panel. 

Each article has a title appearing as bold printed header, a body text and a publication date. 
The chronologically last three articles indicated as **Published** are shown with the newest 
article on top. The body text also allows basic HTML tags like:
 
- line breaks `<br>`
- horizontal lines `<hr>`
- `<b>bold</b>` style 
- `<i>italic</i>` style 
- `<a href=”http://destination.url” target=”_blank”>Link Text</a>` would add a hyperlink with the respective destination, opened in a new window. 