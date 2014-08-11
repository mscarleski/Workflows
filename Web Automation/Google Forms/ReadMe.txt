Task: Create a WorkFlow that collect all the information from the following Google Form 

https://docs.google.com/a/deskperience.com/forms/d/1PSzuXeTkBhaHVdBnkU-N50vGp05el1rXhRoHlao5klw/viewform?c=0&w=1
and put all these information in a Excel sheet.

How to do it?
Well our solution is the following:
Using the latest version of UiPath Studio we built a data table that has as columns all the names of the 
sections from the Form ( eg. First Name , Gender , Birthplace and so on ).
The next step is to use the new activity of UiPath 7.5 "Monitor Events". This function listens to a list a trigger 
and executes a handler every time one of the actions is triggered. Pay attention at the properties of this function
because this function is setup to repeat forever. In our example we use a variable to stop the workflow at only 3 reps.
In "Monitor events" , after the user click the button "Submit" , the workflow collect all the information using the function 
"Get Value" . This function works only for text sections like "First Name" ,"Profession" ... for multiple choice, check box 
and date we will use another function named "Get Attribute". For date the attribute of the function is "selecteditem" 
and the function returns a string but for check box and multiple choice the attribute is "checked" and pay attention 
on the TypeArgument , it should be setup on Boolean. For the RelationShip Section , there are 3 possibilities
and only one option. First we check if he or she is single , if this is false maybe he/she is in a relationship and
if it false again he/she is certainly married.
For the "In which industry have you worked before ? " section it might be one element checked or many so we have to check 
every radio button. If the attribute value ( Get attribute/Properties ) it's true , then a string variable called "prevwork" took the
name of the working industry that is checked. 
For instance if Utilities and Retail are checked, the variable "ischeckedUtilities" and "ischeckedRetail" are true then the 
variable prevwork took the name " Utilities Retail".
Finally we add a data row with all these information in data table and copy everything from data table in a Excel. The last FlowDecision if used to stop the workflow after 3 reps.
