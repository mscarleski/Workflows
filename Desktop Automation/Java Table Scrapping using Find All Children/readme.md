Task

Extract the first name and the sport from a Java App Table.
For Java Find All Children of the table element should be used for every column we want to scrape data from

Steps  

- create a datatable to store the results
- Find All Children for the first column in datatable
```
Filter="<java role='label' tableCol='0' />"
```
- add a For Each Child activity. Inside of it add a new row in our datatable and the corresponding data scraped. 
- Find All Children for the third colum in the datatable
```
Filter="<java role='label' tableCol='2' />"
```

- add a For Each Child activity. Write in our datatable the scraped data.
- output the results in a csv


