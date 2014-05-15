Task

Extract the first name and the sport from a Java App Table.
For Java Find All Children of the table element should be used for every column we want to scrape data from

Steps  

1. create a datatable to store the results
2. Find All Children for the first column in datatable
```
Filter="<java role='label' tableCol='0' />"
```
3. add a For Each Child activity. Inside of it add a new row in our datatable and the corresponding data scraped. 
4. Find All Children for the third colum in the datatable
```
"<java role='label' tableCol='2' />"
```

5. add a For Each Child activity. Write in our datatable the scraped data.
6. output the results in a csv


