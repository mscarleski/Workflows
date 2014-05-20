Task

This sample automates an application via Citrix or Remote Desktop Connection.

Steps

1. On the Remote Dektop Connection open the expenseit application 
2. Start Recorder-> Step By Step and "record" the following actions
3. Click Image ["Create Expense Report"]
4. Click Image ["Add Expense"]
5. Click Image ["(Expense Type)"] in order to position the cursor on the new entry line 
6. Repeat folowing actions: Send Hotkey ["Ctrl+A"]  for selecting the text, Type the desired value, Type Tab for moving to the next cell
7. For scraping the total value we add a Scrape Screen activity
8. Click Image ["OK] and Click Image ["OK]
9. We add a Regex activity for parsing the result text (remove "Total Expenses ($):" text.
	 

