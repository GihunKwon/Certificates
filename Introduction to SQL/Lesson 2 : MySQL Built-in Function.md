## 2.1 MySQL Built-in Function
<br/>

### Practice
- check the databases
1. show databases;
2. use world;
3. show tables;
4. select * from city;
5. describe city;
<br/>

- create a new database and a table
1. create database sql_intro;
2. show databases;
3. USE sql_intro;
<br/>

1. create table emp_details(Name varchar(25), Age int, Sex char(1), doj date, city varchar(15), salary float);
2. describe emp_details;
3. insert into emp_details
    values("Jimmy",35,"M,"2005-05-30","Chicago",70000),(.....),(.....);
4. select * from emp_details;
<br/>

1. DISTINCT
2. COUNT()
3. ALIAS (AS)
4. SUM()
5. AVG()
6. WHERE
7. OR
8. IN (....)
9. BETWEEN
10. Comparison (=,>,<,...)
11. GROUP BY
12. ORDER BY
13. LENGTH()
14. REPEAT('',number)
15. UPPER()
16. LOWER()
17. CURDATE()
18. DAY()
19. NOW()
20. CHARACTER_LENGTH('')
21. CONCAT()
22. REVERSE()
23. REPLACE("Original data","Keyword","Replacement")
24. ltrim()
25. rtrim()
26. POSITION("Keyword" in "TEXT")
27. ASCII("Letter")
<br/>