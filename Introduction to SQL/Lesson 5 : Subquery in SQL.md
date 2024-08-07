## 5.1 Subquery in SQL
<br/>

### What is Subquery?
- A subquery is a select query that is enclosed inside another query. The inner select query is usually used to determine the results of the outer select query.
<br/>

### Types of Subqueries
1. SELECT
    - most commonly used
2. INSERT
    - the data returned from the subquery is inserted into another table
3. UPDATE
    - columns in a tabel can be updated when using a subquery
4. DELETE
    - 
<br/>

<br/><br/>

### Triggers in DBMS
<br/>

### What are Triggers in SQL?
- A trigger is a user-defined SQL command that is invoked automatically in response to an event such as insert, delete or update.
<br/>

### Practice
<br/>

* before insert trigger
DELIMITER //
<br/>
CREATE TRIGGER age_verify # trigger name
BEFORE INSERT ON customers # table name
FOR EACH ROW #
IF NEW.age < 0 THEN SET NEW.age = 0; 
END IF; //
<br/><br/>

* after insert trigger
DELIMITER //
CREATE TRIGGER check_null_dob
AFTER INSERT ON customers1
FOR EACH ROW
BEGIN
IF NEW.birthdate IS NULL THEN 
    INSERT INTO message (messageId,message)
    VALUES (NEW.id, CONCAT('Hi',NEW.name,'please update your date of birth'))
END IF;
END //
DELIMITER;
<br/>

???????????