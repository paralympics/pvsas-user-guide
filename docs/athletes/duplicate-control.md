# Duplicate Control

The duplicate control functionality is used to generate PDF reports indicating possible duplicate
entries in PVSAS. The search is customisable and automatically restricted by user data access.
Additionally, a merging tool allows to easily remove duplicates by merging relevant information
to a single profile.

The search criteria are specified by the following fields:

| **Field**                                           | **Format**             | **Comments**                                         |
| --------------------------------------------------- | ---------------------- | ---------------------------------------------------- |
| **Sport**                                           |                        | Defaults to ParaVolley                               |
| **Member Federation**                               | drop down [federation] |                                                      |
| <span class="table-header">Equality Criteria</span> |                        |                                                      |
| **Family Name (passport)**                          | tick box               | default selections if no other criteria are applied. |
| **Given Name (passport)**                           | tick box               | default selections if no other criteria are applied. |
| **National Federation**                             | tick box               |                                                      |
| **Gender**                                          | tick box               |                                                      |
| **Date of Birth**                                   | tick box               |                                                      |
| **Passport/ID Card No**                             | tick box               |                                                      |

The criteria work in conjunction – the search only returns items that are equal on all selected
criteria, within any possible restriction by NF and/or sport.

Clicking **Search** opens a new tab in the browser with a PDF of the matches. Except for sport, all
personal data which can be searched is also displayed here, along with the career status of the
athlete.

When duplicates are found, it is recommended to merge all data from one profile the other and
delete the obsolete entry to keep the system clean.