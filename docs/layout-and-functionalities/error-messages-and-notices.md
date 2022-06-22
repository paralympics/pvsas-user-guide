# Error Messages and Notices

The application informs the user about the success or error on his actions in any screen or data 
set. These messages appear at the top of the application, underneath the primary menu bar. 

### Success

Dark green notices on green background report on the successful actions like submission of 
data, creation, update, or deletion of a data set etc.

<figure>
    <img src="_img/inline/flash-message-success.png" alt="Flash message for successful action" class="screenshot" >
</figure>

### Error

On the other hand, dark orange messages indicate that the intended action was not 
successfully performed to prevent that incorrect data are stored or data sets removed which are 
associated with other important data sets.

<figure>
    <img src="_img/inline/flash-message-error.png" alt="Flash message for error" class="screenshot">
</figure>

### Information

A yellow warning message is displayed when the user’s action could cause database integrity 
issues. Usually, the user’s action is not carried out. 

<figure>
    <img src="_img/inline/flash-message-info.png" alt="Flash message for information" class="screenshot" >
</figure>

Notices to the user vanish after a short time; they can also be clicked on to remove them 
immediately.

Reasons for an error are manifold, the most common errors are:

- Mandatory fields were not filled.
- Attached files do not meet the requirements ([File Attachments](layout-and-functionalities/file-attachments.md)). 
- The field value has not the right content or format ([Data Fields](layout-and-functionalities/data-fields.md)). 
- An essential data set (like an athlete) is attempted to be deleted although other essential 
data sets (like licenses or classifications) are associated. 
- User credentials were incorrect on login attempt ([Security and Passwords](layout-and-functionalities/access.md#security-and-passwords)).

All individual errors are shown at once after data submission. In the data set detail pages, the 
values that the user changed or included are kept, except for selected files from the user’s local 
computer system for security reasons.

Most of the cases can be resolved by the user reading and applying the instructions of the error 
message. When an unclear or cryptic error message appears, please contact the IPC SDMS 
Administrator for explanation and support to fix the issue.  