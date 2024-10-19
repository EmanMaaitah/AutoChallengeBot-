# OBJECTIVE 
The project talks about a [challenge](https://rpachallenge.com/) created by the ui path team to input data from a spreadsheet into the form fields on the screen.
The idea of ​​the project is to track the input field based on its position every time the page is updated to move to the next stage.The goal of the project is to learn how to use [the Targets and Anchors selectors](https://docs.uipath.com/studiox/standalone/2022.4/user-guide/about-targets-and-anchors) . Anchors used with unstable selector, In addition to the [strict and fuzzy selector](https://docs.uipath.com/activities/other/latest/ui-automation%22/advanced-descriptor-configuration).
## manually
1) Excel 
2)  Data Transfer
3)  Website


<img src="https://github.com/user-attachments/assets/b534809f-bf79-4585-b55a-ad910218452e" width="250">

# TECHNICAL REQUIREMENTS
## Using Excel Activities
1) [Excel Process Scope](https://docs.uipath.com/activities/other/latest/productivity/excel-process-scope-x)
2) [Use Excel File](https://docs.uipath.com/activities/other/latest/productivity/excel-application-card)
3) [Read Range](https://docs.uipath.com/activities/other/latest/productivity/excel-read-range)

## Using Data Table Activities
1) [Output Data Table](https://docs.uipath.com/activities/other/latest/workflow/output-data-table)
2) [For each row in Data Table](https://docs.uipath.com/ACTIVITIES/other/latest/workflow/for-each-row)

## UI Automation Activities
1) [Use Application/Browser](https://docs.uipath.com/activities/other/latest/ui-automation%22/n-application-card)
2) [Navigate Browser](https://docs.uipath.com/activities/other/latest/ui-automation/n-navigate-browser)
3) [Keyboard Shortcuts](https://docs.uipath.com/activities/other/latest/ui-automation%22/n-keyboard-shortcuts)
4) [Click](https://docs.uipath.com/activities/other/latest/ui-automation%22/click)
5) [Log Message](https://docs.uipath.com/activities/other/latest/workflow/log-message)
6) [Type Into](https://docs.uipath.com/activities/other/latest/ui-automation%22/type-into)
7) [Get Text](https://docs.uipath.com/activities/other/latest/ui-automation%22/n-get-text)
8) [Message Box](https://docs.uipath.com/activities/other/latest/workflow/message-box)

# PROCEDURES

<img src="https://github.com/user-attachments/assets/1c12c3f5-807d-4094-9109-0bf7ee3578f0">

inside the Excel file put the extention 


<img src="https://github.com/user-attachments/assets/c056c9b1-fba0-415d-a9b1-3989a6fcd398" width="350">

.


<img src="https://github.com/user-attachments/assets/f5146946-45dd-4bac-8f23-732a950ff23a" width="350">


The Read Range activity save data in Excel in Data Table Format, we use the output data taple to transfer the type of data from Data table to string so the message box can print it.

<img src="https://github.com/user-attachments/assets/fca335d6-269c-49e8-89af-6e2bcdbf1196" width="350">


.


<img src="https://github.com/user-attachments/assets/2369ef5d-c011-4630-ae50-1c5bf1e2ebee" width="350">


Navigate browser is used to refresh website pages, Keyboard Shortcuts (Ctrl+0) To avoid any page enlargement.

<img src="https://github.com/user-attachments/assets/18f273ae-ebd4-4b4c-9919-31466882a034" width="350">



.

<img src="https://github.com/user-attachments/assets/801637f2-7c3e-4243-8206-d30053ad0f78" width="350">


The variable created by Read range is called and through for each all rows will be read.




<img src="https://github.com/user-attachments/assets/26ac7129-4bb1-44b2-a207-fd0d54b29869" width="350">


The current row is a variable that is only specific to the for each scope and we cannot call it outside of it




<img src="https://github.com/user-attachments/assets/ab5236d9-105a-45c1-9f6f-3e7c5c88da6e" width="350">



The strict selector will be deactivated in the selection options because it does not accept flexibility and moving fields. The innertext attribute will also be added to the fuzzy selector.

<img src="https://github.com/user-attachments/assets/327f23ff-8f6c-45f1-a20a-bda404a0239f" width="350">


.

<img src="https://github.com/user-attachments/assets/7a711a82-5fb7-439b-a51d-7109d6dc23ed" width="350">


Finally, the result is taken and sent to the user.

