# SQL Tutorial (or) SQL Cheatsheet
* The only SQL tutorial/cheatsheet you'll ever need. 


![img](images/sql.jpg)

## SQL (Structured Query Language)
### What is SQL?
* Language used to create, access and manage databases.
* Trivia: It became an ANSI/ISO (American National Standard Institute and International Organization for Standardization) .

### Requirements for SQL
* RDBMS (Relational Database Management System) like MS Access, MySQL, SQL Serer, Oracle, IBM DB2.
* Server-side scripting language such as PHP, ASP
* SQL
* HTML/CSS for front-end visualization

### Basic Terminologies 101
* Table (Collection of rows and columns)
* Field/Fields
* Rows/Record

## SQL Commands

* #### SQL Select

Semicolon is required to seperate different SQL commands. SQL is case in-sensitive.
```
SELECT * FROM Customers;
```
```
SELECT column1, column2 FROM table_name;
```
* #### SQL SELECT DISTINCT

Displays only the unique results, without duplicates.
```
SELECT DISTINCT * FROM CUSTOMERS;
```
```
SELECT DISTINCT CustomerName, ContactName FROM CUSTOMERS;
```
```
SELECT COUNT (DISTINCT CustomerName) FROM CUSTOMERS;
```
* #### SQL WHERE CLAUSE
```
SELECT * FROM CUSTOMERS WHERE CUSTOMERID IS 1;
```
```
SELECT * FROM CUSTOMERS WHERE CITY IS "London";
```
* #### SQL AND, OR, NOT CLAUSE
```
SELECT * FROM CUSTOMERS WHERE CITY IS "London" AND CUSTOMERID IS 4;
```
```
SELECT * FROM CUSTOMERS WHERE CITY IS "London" OR CUSTOMERID IS 3;
```
```
SELECT * FROM CUSTOMERS WHERE NOT CUSTOMERID IS 3;
```





