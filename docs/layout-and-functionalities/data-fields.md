# Data Fields

Search criteria forms, entity detail pages and similar generally are simple HTML forms and are 
composed of free text fields, drop down menus, radio, and tick boxes. Each field is labelled 
according to its value behind. Some fields have prepended a small red question marker icon 
which contains more explanations and regulations about the field and its content when cursor is 
moved over.

PVSAS has a few additional functionalities or tools behind the fields the user must be aware of:

- **Mandatory Fields** – Fields with a light-yellow background are mandatory. Leaving such a 
field blank upon submission will cause an error, and the data set won’t be saved unless 
the field has a valid value. 
- **Value Validity Control** – Each field is subject to a set of specific rules. These rules might 
consider value length (number of characters), value type (integer, float, text, …) or even 
specific value formats (dates, NPC Code, …). On validation failure, an error is thrown, 
and the related field is displayed in red. 
- **Files** – When a file upload becomes necessary, the file is checked against the maximal 
file size (in bytes) and file format (photos, PDFs). Photos are additionally reviewed for 
potential limits in image size (in pixels). 
- **Character Sets** – Names and other information shall be written in English language. Only 
the English alphabet and a few characters (e.g. hyphen) are allowed. Diacritics must be 
removed, and non-English letters must be transcribed (e.g. ä -> ae). 
- **Date Field** – The standardized date field format is yyyy-mm-dd (year – month – day). 

<img src="_img/inline/date-field.png" alt="Date Field" class="center inline-screenshot">

When a date field (e.g., athlete’s date of birth) is selected, a small calendar tool 
appears to automatically allow the user to select the correct date. Drop down boxes on 
top opens the respective calendar by month and year. 
The buttons <img src="_img/inline/date-field-left.svg" alt="Left Scroll" class="inline svg-small"> 
and <img src="_img/inline/date-field-right.svg" alt="Right Scroll" class="inline svg-small"> 
scroll through the calendar by month. The selected date will be highlighted. This small window 
closes automatically when a date is selected, the button **Done** is clicked or another 
field is selected. In some date fields, minimum and maximum dates are set up. 
The calendar tool for those fields only displays the acceptable date range. 