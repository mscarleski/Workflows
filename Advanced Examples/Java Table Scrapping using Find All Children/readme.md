Task

Extract FirstName and Sport columns from a table inside a Java App.

The way to do this in Java is by using FindAllChildren activity.

Steps  

- create a datatable to store the results
- FindAllChildren for the FirstName column in datatable
```
Filter="<java role='label' tableCol='0' />"
```
- add a ForEachChild activity. Inside of it add a new row in our datatable and the corresponding data scraped. 
- FindAllChildren for the Sport colum in the datatable
```
Filter="<java role='label' tableCol='2' />"
```

- add a ForEachChild activity. Write in our datatable the scraped data.
- output the results in a csv


