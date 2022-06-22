# Defects

Application defects, also known as **‘bugs’**, prevent the user from using the system. They are either 
of syntactical or semantic in nature. Syntax errors will produce a cryptic error message to the end 
user or just a browser error, sometimes with error code 500. 

Semantic errors refer to a wrong implementation of a business process. While the application itself 
works, the data stored, or results calculated differ from the expectations or logical outcome.

In both cases, the NPC shall immediately register this defect. 

The registration process is similar to change requests as explained in [Change Requests](database-issue-tracker/change-requests.md). 
Defect reports automatically have high priority and are based on user experience. The IPC considers and 
fixes each defect at their earliest convenience so that a *completion date* is not necessary. However, 
especially for defects it is of high importance to describe the steps until the error appeared as 
detailed as possible so that the developer in charge can reproduce it, find the issue, and fix it 
immediately. A screenshot of the error messages or screen appearing should be uploaded that often 
helps much more than long explanations. 

Like change requests, each submission of a defect triggers an automatic email notification to the 
IPC Sports IT team for their immediate awareness. Once the issue is fixed, the status will be changed 
to *Completed* and the detector of the issue personally informed.