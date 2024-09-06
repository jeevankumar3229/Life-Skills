# SQL
Structured Query Language (SQL) is a domain-specific language used to manage data, especially in a relational database management system (RDBMS). It is particularly useful in handling structured data, i.e., data incorporating relations among entities and variables. Introduced in the 1970s, SQL offered two main advantages over older read–write APIs such as ISAM or VSAM. Firstly, it introduced the concept of accessing many records with one single command. Secondly, it eliminates the need to specify how to reach a record, i.e., with or without an  index.    Originally based upon relational algebra and tuple relational calculus, SQL consists of many types of statements, which may be informally classed as sublanguages, commonly: Data query Language (DQL), Data Definition Language (DDL), Data Control Language (DCL), and Data Manipulation Language (DML). The scope of SQL includes data query, data manipulation (insert, update, and delete), data definition (schema creation and modification), and data access control. Although SQL is essentially a declarative language (4GL), it also includes procedural elements.

## Predefined data types in SQL
### Character types
1. Character (CHAR)
2. Character varying (VARCHAR)
3. Character large object (CLOB)
### National character types
1. National character (NCHAR)
2. National character varying (NCHAR VARYING)
3. National character large object (NCLOB)
### Binary types
1. Binary (BINARY)
2. Binary varying (VARBINARY)
3. Binary large object (BLOB)
### Numeric types
1. Exact numeric types (NUMERIC, DECIMAL, SMALLINT, INTEGER, BIGINT)
2. Approximate numeric types (FLOAT, REAL, DOUBLE PRECISION)
3. Decimal floating-point type (DECFLOAT)
### Datetime types 
1. DATE
2. TIME
3. TIMESTAMP
### Interval type 
1. INTERVAL
### Boolean type
1. Boolean


## Basic SQL Commands
### 1. SQL CREATE DATABASE
SQL CREATE DATABASE statement creates a new database in SQL-based DBMS.  
**Syntax** : CREATE DATABASE database_name;
### 2. List Databases in SQL
SHOW DATABASES statement list all the databases.  
**Syntax** : SHOW DATABASES;
### 3. SQL DROP DATABASE
SQL DROP DATABASE statement is used to delete an existing database from the database management system (DBMS).  
**Syntax** : DROP DATABASE database_name;

### 4. SQL Query to Rename Database
The ALTER command in SQL is used to make changes to a table or database.  
**Syntax** : ALTER DATABASE current_database_name MODIFY NAME = new_database_name;
### 5. SQL Select Database
The USE DATABASE statement is a command in certain SQL-based database management systems that allows users to select and set a specific database as the default for the current session.       
**Syntax** : USE database_name;
### 6. SQL CREATE TABLE
CREATE TABLE command creates a new table in the database in SQL.  
**Syntax** : 
CREATE table table_name
(
Column1 datatype (size),
column2 datatype (size),
.
.
columnN datatype(size)
);
### 7. SQL DROP TABLE
The DROP TABLE command in SQL is a powerful and essential tool used to permanently delete a table from a database, along with all of its data, structure, and associated constraints such as indexes, triggers, and permissions.  
**Syntax** : DROP TABLE table_name;
### 8. SQL DELETE Statement
SQL DELETE is a basic SQL operation used to delete data in a database.  
**Syntax** : DELETE FROM table_name WHERE some_condition;
### 9. ALTER (RENAME) in SQL
SQL ALTER TABLE is a command used to modify the structure of an existing table in a database.  
**Syntax** : ALTER TABLE table_name RENAME TO new_table_name;

### 10. SQL ALTER TABLE
SQL ALTER TABLE command can add, delete, or modify columns of an existing table.  
**Syntax** : ALTER TABLE table_name clause column_name datatype;
### 11. SQL SELECT Query
The SELECT statement in SQL is used to fetch or retrieve data from a database. It allows users to access the data and retrieve specific data based on specific conditions.  
**Syntax** : SELECT column1,column2…. FROM table_name ;
### 12. SQL INSERT INTO Statement
The INSERT INTO statement is a fundamental SQL command used to add new rows to a table in a database. It allows for the insertion of data either by specifying the column names along with the values or by providing values for all columns in the table.  
There are two primary syntaxes of INSERT INTO statements depending on the requirements. The two syntaxes are:  
1. Only Values  
**Syntax** : INSERT INTO table_name VALUES (value1, value2, value);  
2. Column Names And Values Both  
**Syntax** : INSERT INTO table_name (column1, column2, column3) VALUES ( value1, value2, value);   

## SQL Aggregate functions
### 1. SQL COUNT() Function  
The COUNT() function provides the number of rows that match a specified condition. This function is particularly useful for understanding the volume of data entries and identifying trends based on countable metrics.  
**Syntax** : SELECT COUNT(column_name) FROM table_name WHERE condition;
### 2. SQL AVG() Function  
The AVG() function provides the average value of a numeric column.  
**Syntax** : SELECT AVG(column_name) FROM table_name WHERE condition;  
### 3. SQL SUM() Function  
The SUM() function provides the total sum of a numeric column.  
**Syntax** : SELECT SUM(column_name) FROM table_name WHERE condition;  
### 4. SQL MIN() Function
SQL MIN() function returns the smallest value in the column.  
**Syntax** : SELECT MIN(column_name) FROM table_name WHERE condition;  
### 5. SQL MAX() Functions  
SQL MAX() function returns the largest value in the column.  
**Syntax** : SELECT MAX(column_name) FROM table_name WHERE condition;



## SQL Joins 
### 1. SQL Inner Join
The INNER JOIN clause in SQL is used to combine multiple tables and fetch records that have the same values in the common columns.  
**Syntax** : SELECT columns FROM table1 INNER JOIN table2 ON table1.column_name = table2.column_name;  
### 2. SQL LEFT JOIN
SQL LEFT JOIN command returns all records from the tableA and matching records from the tableB. If there is no matching record in the tableB, the tableB records will contain NULL values.  
**Syntax** : SELECT column_name(s) FROM tableA LEFT JOIN tableB ON tableA.column_name = tableB.column_name;  
### 3. SQL RIGHT JOIN  
SQL RIGHT JOIN returns all records from the tableB, and the matching records from the tableA in the results set.  
**Syntax** : SELECT column_name(s) FROM tableA RIGHT JOIN tableB ON tableA.column_name = tableB.column_name;
### 4. SQL FULL JOIN  
SQL FULL JOIN or FULL OUTER JOIN returns a new table containing all records of the table1 and table2 on a match.  
**Syntax** : SELECT columns FROM table1 FULL OUTER JOIN table2 ON table1.column = table2.column;
### 5. SQL CROSS JOIN  
SQL CROSS JOIN returns all the records from the table1 and table2. CROSS JOIN returns a combination of each row in the table1 paired with each row in the table2.  
**Syntax** : SELECT * FROM table1 CROSS JOIN table2;  
### 6. SQL Self Join  
A Self Join is a regular join that is used to join a table with itself.  
**Syntax** : SELECT columns FROM table AS alias1 JOIN table AS alias2 ON alias1.column = alias2.column;


## References
1. [Wikipedia](https://en.wikipedia.org/wiki/SQL)
2. [GeeksforGeeks](https://www.geeksforgeeks.org/sql-tutorial/)