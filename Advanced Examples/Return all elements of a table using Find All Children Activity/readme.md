Task

Return all TR elements of a table you have to use Find Children activity.

Steps  

1. Ad a Find All Children Activity
2. Select the entire table using the Selector property
3. Set the Scope property to "Find Descendents" 
4. Set in the filter property partial selector that identifies the TR. This selector should not include the table selector.
5. The final For Each activity iterates through the elements of the output collection and highlights them
