# Search Forms & Results Matrix

Each section handling one data entity of PVSAS, e.g. sports, events, federations or athletes, has 
a search functionality to target the user’s data.

<figure>
    <img class="screenshot" src="_img/figures/2.9-search-results-matrix.png" alt="Search Results Matrix">
    <figcaption>Figure 2.9 - Search Results Matrix - Application  (Application Settings > Config > App News)</figcaption>
</figure>

The search page in turns offers a results matrix with an input row for the search criteria. When a 
new section is opened, the current criteria are automatically applied, along with the user’s 
permission criteria (for example, the athletics federation will only receive search results about 
athletes registered in that sport), and the results are displayed. Generally, the search returns all
relevant results when initially opened, and the current criteria can then be modified. When 
changing the drop-down boxes, the search is automatically reset, while when changing text 
boxes, users must refresh or press the **Return** key on their keyboard.

Users specify their search parameters by entering text or selecting items from the dropdown 
search fields. Each search field only allows for entries with fewer or the same number of 
characters defined in the database structure. 

In the result of each search conducted the information is displayed in columns and rows (a 
search results matrix). Users may manipulate the width of each column, change the order of the 
columns by drag-and-drop and sort by a column according to need. The current sorting column 
is indicated by a downwards (ascending) or upwards (descending) pointing triangle.

If you wish to remove or clear a search criterion, click the cross next to its drop-down box or text 
field. The application treats most text searches as asking for text strings that ‘contain’ the 
supplied text, rather than exact matches.

The footer consists of several icons for handling the data or scroll through the full set of data.

| **Icon**                                                                                | **Description**                                                                                                                     |
| :-------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------- |
| <img src="_img/inline/icon-delete.svg" alt="Delete" class="inline svg-large"> | Deletes the selected row(s). On attempt to delete data which is related to other information or entities, an error message appears. |
| <img src="_img/inline/icon-reload.svg" alt="Reload" class="inline svg-large">                    | Reloads the grid.                                                                                                                   |
| <img src="_img/inline/icon-filter-remove.svg" alt="Reset" class="inline svg-large">               | Clears the search parameters.                                                                                                       |
| <img src="_img/inline/icon-format-columns.svg" alt="Column" class="inline svg-large">             | Manipulate order and number of columns supported by a small interface.<span class="asterisk">*</span>                               |
| <img src="_img/inline/icon-excel-download.svg" alt="Export" class="inline svg-large">             | Exports all data based on search criteria and column selection and order into an Excel file.                                        |
| <img src="_img/inline/icon-tools.png" alt="Tools" class="inline icon-set">              | Tools to select matrix pages.                                                                                                       |
| <img src="_img/inline/icon-first.png" alt="First" class="inline icon-set">              | Go to first page.                                                                                                                   |
| <img src="_img/inline/icon-previous.png" alt="Previous" class="inline icon-set">        | Go to previous page.                                                                                                                |
| <img src="_img/inline/icon-next.png" alt="Next" class="inline icon-set">                | Go to next page.                                                                                                                    |
| <img src="_img/inline/icon-last.png" alt="Last" class="inline icon-set">                | Go to last page.                                                                                                                    |
| <img src="_img/inline/icon-direct.png" alt="Direct" class="inline icon-set">            | Direct page selection: change page number and press **Enter**.                                                                      |
| <img src="_img/inline/icon-rows.png" alt="Rows" class="inline icon-set">                | Changes the number of rows per page.                                                                                                |
| <img src="_img/inline/icon-current.png" alt="Current" class="inline icon-set">          | Shows current position and total data rows based on search criteria.                                                                |

<p class="footnote">
    <small><span class="asterisk">*</span>Hidden columns which do not fit in the default view can be added here if necessary.</small>
</p>

Each row in the matrix represents one data set with some basic information. 
- That row the mouse cursor is just selecting is highlighted in light green. 
- To select a row for deletion or other actions in specific sections, the user ticks the box on 
the left-hand side. Selected rows are highlighted in light blue.
-  When a data row is clicked, the detail page opens to review and manipulate. Some 
screens do not have a detail page; in that case, clicking selects the row.

<figure>
    <img class="screenshot" src="_img/figures/2.10-selecting-rows-in-a-grid.png" alt="Selecting rows in a grid">
    <figcaption>Figure 2.10 - To select all rows, click the checkbox in the header row</figcaption>
</figure>

Underneath the search results matrix, three buttons duplicate the functionality of icons in the 
matrix footer, namely the Delete button (same as <img src="_img/inline/icon-delete.svg" alt="Delete" class="inline svg-small">), 
the **Grid Export** button (same as <img src="_img/inline/icon-excel-download.svg" alt="Export" class="inline svg-small">), and 
the **Clear Filter** button (same as <img src="_img/inline/icon-filter-remove.svg" alt="Clear Filter" class="inline svg-small">).

After opening the detail page, you can go back by clicking **Back to Grid** at the upper right corner of the detail page. 
These buttons re-apply the search criteria and opens the previous search results matrix page. Additional buttons 
on the detail page open a blank form to create a new data set (**Add New X or New**), save, refresh, delete, or 
clear the loaded detail page. Further buttons designed for a specific detail page are described in the respective 
sections of this guide.

When moving the cursor over the <img src="_img/inline/icon-modifier-info.svg" alt="Modifier Information" class="inline svg-small"> 
icon, information about who created the data set at which time and who edited the data set the last time. 