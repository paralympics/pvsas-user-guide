When administrating large numbers of athlete data, it is often a good idea to print database 
extracts as PDF or Excel files in a report. These reports can be generated as **Grid Export** 
from each search table, but the specifically designed report section of PVSAS combines data 
from various tables for more comprehensive reporting.

The Report section is available to both NPC and NF users. NF users can only download data
related to their sport’s own athletes.

# Classification Master List

The *Classification Master List* is the main report produced by PVSAS, and the one with the most 
customisable options. It can be used to prepare classification schedules for competitions, get 
an overview of all athletes from a national federation, club, and/or sport. A classification report 
can only be produced for one sport at a time; therefore, the Sport drop-down box is compulsory. 
The user must be aware that athletes with pseudo-class **‘N/A’** are excluded from all reports.

The PDF reports generated in PVSAS are generic across all sports. They only include the athlete 
data and some basic information like class, class status, year of review, date of classification 
and classification level (national/ international) for each athlete.

## Competition Search

It is possible to specify the competition/ classification event code for the search 
([Competitions](calendar/competitions.md)). This produces a report for all athletes registered 
to that event through the sport-specific assignment page 
([Assigning Athletes and Classifiers](calendar/competitions.md#assigning-athletes-and-classifiers)), 
particularly useful for the preparation of classification schedules. If the competition code is not 
set, all athletes from the database are considered based on the other criteria.

## Other Options

A comprehensive table of all search options follows.

| **Field**                                         | **Format**             | **Comments**        |
| ------------------------------------------------- | ---------------------- | ------------------- |
| <span class="table-header">Core Parameters</span> |                        |                     |
| **Discipline**                                    | drop-down [value list] | Sitting or Standing |

## PDF Export

PDF reports are printed in landscape format, with a set number of columns varying from 
sport to sport when you click the *Open as PDF* button. The report is also timestamped 
and verified with the official logos of World ParaVolley.

From the left, each row includes personal data – Athlete ID, family name, given name, 
gender, date of birth – the athlete’s current class, the class status, and the year of 
review. If the athlete has different classes for different events and/or disciplines, 
this is also shown next to the class name.

The classification master list report tries to find any inconsistencies in the classification 
of athletes, e.g. an athlete in a single-class sport like alpine skiing has two classes currently 
registered. Such inconsistencies are indicated as red message underneath the respective athlete 
and should be immediately fixed.

## Excel Export

The Excel export is similar to the PDF but meant for internal use and analysis. The athletes
are listed in rows by the sorting order specified; as there is no restriction on horizontal space
in a spreadsheet, all classification data (profile and file upload information) is displayed in a
single row.

This also allows enough space to include the additional columns with registration status and
uploaded form data; see [Classification Master List](reports/classification-master-list.md#other-options) 
how to include specific information. In Excel, you may manipulate the report with your own search filters, 
sorts, etc., but this is spreadsheet-specific and outside the scope of this manual.

## Classification Master List Widget

For PVSAS, a publicly accessible widget is available that can be accessed on

<p class="text-center">
  <a href="https://pvsas.worldparavolley.org/web" target="_blank">https://pvsas.worldparavolley.org/web</a>
</p>

<figure>
    <img src="_img/figures/6.1-classification-master-list-widget.png" alt="Classification Master List Widget" class="screenshot" >
    <figcaption>Classification Master List Widget</figcaption>
</figure>

The widget has a maximum width of 720px and is intended to be included via an HTML `<iframe>` 
into any webpage. The public visitor selects the sport and decides on the format as they are 
a browser version in HTML, a PDF version, an Excel sheet, and the underlying XML as possible 
outputs.

It is also possible to publish links to these reports on any webpage which might be useful to 
give the public a direct insight into the current classification master lists of World ParaVolley 
as all data are directly extracted live from PVSAS. The format of the link is

<p class="text-center"><b>https://pvsas.worldparavolley.org/web/cml/format/[:format]</b></p>

with

[:format] as desired output format of the report. Allowed values are:
- *html* - the HTML version of the master list
- *pdf* - the PDF version
- *excel* - an Excel version (xlsx extension, Excel 2007+)
- *xml* - a proper data exchange format based on the standard of the Olympic Data Feed 
  (ODF) but with several application specific adjustments and codes

In comparison to the PDF reports of the password-protected PVSAS environment 
(see [PDF Export](reports/classification-master-list.md#other-options)), the 
reports generated by this widget are designed for public use. Date of birth is 
removed and replaced by the year of birth, some basic error indicators like 
duplicated classes for single-class sports are removed and some specific 
classification profile fields, like the extensions in swimming are included 
upon request of the responsible federation.