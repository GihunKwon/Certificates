## 10.1 SQL Interview Questions
<br/>

### Questions
1. state the difference between WHERE and HAVING in SQL
    - WHERE
        - used to filter the records based on the specified condition
        - cannot have aggregate functions
        - implemented on rows
    - HAVING
        - used to filter the records from groups based on specified conditions
        - can operate on aggregate functions
        - implemented on columns

2. how is DROP different from TRUNCATE
    - DROP
        - remove table definition and its contents
        - the view of the table does not exist
        - integrity constraints will be removed
    - TRUNCATE
        - delete all the rows from the table
        - the view of the table exists
        - integrity constraints will not be removed

3. coding test

4. coding test

5. coding test

6. coding test

7. what is the use of DATEDIFF function in SQL
    - return the number of days between two date, datetime, or timestamp values

8. coding test

9. coding test

10. coding test

11. coding test

12. coding test

13. coding test

14. coding test

15. coding test

16. how does SELF JOIN work
    - the SELF JOIN joins a table to itself
    - the table must contain a column(x) that acts as the primary key and a different column(y) that stores values that can be matched up with the values in column x

17. coding test

18. coding test

19. coding test

20. coding test

21. coding test

22. what is the difference between PRIMARY KEY and FOREIGN KEY
    - PRIMARY KEY
        - uniquely identify a record in the table
        - cannot accept null values
        - only one primary key in a table
    - FOREIGN KEY
        - field in the table that is primary key in another table
        - can accept null values
        - more than one foreign key in a table

23. what is the difference between PRIMARY KEY and UNION
    - PRIMARY KEY
        - only one primary key in a table
        - cannot accept null values
        - create clustered index
    - UNION
        - can be more than one unique key in a table
        - can accept null values
        - create non-clustered index

24. what is a check constraint in SQL
    - the check constraint is used to limit the values that can be inserted into a column

25. coding test

26. coding test

27. coding test

28. coding test

29. coding test

30. coding test
<br/>