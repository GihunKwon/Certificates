## 3.1 Group By and Having
<br/>

### Group By in SQL
- group records into summary rows and returns one record for each group
<br/>

### Practice
1. show databases;
2. use sql_intro;
3. show tables;
4. create table employees (Emp_Id int primary key, Emp_name varcarh(25), Age int, Gender char(1), Doj date, Dept varchar(20), City varchar(15), Salary float);
5. describe employees;
6. insert into employees values (.....),(.....);
7. select dept,avg(age) from employees group by dept;
    - avg, sum, count..
8. select year(doj) as year, count(emp_id) from employee group by year(doj);
<br/>

1. create table sales (product_id int, sell_price float, quantity int, state varchar(20));
2. insert into values (.....)(.....);
3. select product_id, sum(sell_price*quantity) as revenue from sales group by product_id;
<br/>

1. create table c_product (product_id int, cost_price float);
2. insert into c_product values (.....),(.....);
3. select c.product_id, sum((s.sell_price - c.cost_price) * s.quantity) as profit from sales as s join c_product as c where s.product_id = c.product_id group by c.product_id;
<br/>

<br/><br/>

### Having in SQL
- operates on grouped records and returns rows where aggregate function results matched with given conditions only
<br/>

### practice
1. select dept, avg(salary) as avg_salary from employees group by dept having avg(salary) > 75000;
2. select city, count(*) as emp_count from employees where city != "Houston" group by city having count(*) > 2;
<br/>