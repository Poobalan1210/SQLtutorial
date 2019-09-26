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
SELECT column1, column2 FROM table_name;
```
* #### SQL SELECT DISTINCT

Displays only the unique results, without duplicates.
```
SELECT DISTINCT * FROM CUSTOMERS;
SELECT DISTINCT CustomerName, ContactName FROM CUSTOMERS;
SELECT COUNT (DISTINCT CustomerName) FROM CUSTOMERS;
```
* #### SQL WHERE CLAUSE
```
SELECT * FROM CUSTOMERS WHERE CUSTOMERID IS 1;
SELECT * FROM CUSTOMERS WHERE CITY IS "London";
```
* #### SQL AND, OR, NOT CLAUSE
```
SELECT * FROM CUSTOMERS WHERE CITY IS "London" AND CUSTOMERID IS 4;
SELECT * FROM CUSTOMERS WHERE CITY IS "London" OR CUSTOMERID IS 3;
SELECT * FROM CUSTOMERS WHERE NOT CUSTOMERID IS 3;
```
* #### Combining AND, OR, NOT
```
SELECT * FROM CUSTOMERS WHERE CustomerID IS 1 AND (CITY IS "London" OR CITY IS "Berlin");
SELECT * FROM CUSTOMERS WHERE NOT COUNTRY IS "Germany" OR (CustomerName IS "Maria Anders" AND CITY IS "Berlin");

```
* #### SQL ORDER BY CLAUSE

Used to order the result either in ascending or descending order
```
SELECT * FROM Customers ORDER BY CONTACTNAME DESC;
SELECT * FROM Customers ORDER BY CUSTOMERID ASC;
```
* #### INSERT INTO 

Used to insert values into columns/fields of the table
```
INSERT INTO CUSTOMERS (CustomerID, CustomerName, ContactName, Address, City, PostalCode, Country) VALUES ('100', 'Sai Adarsh', 'Adarsh', 'Velachery', 'Chennai', '600088', 'India');
INSERT INTO CUSTOMERS (CustomerID, CustomerName, ContactName) VALUES ('100', 'Sai Adarsh', 'Adarsh');

```
* #### NULL CLAUSE

Used to display null or empty
```
SELECT * FROM CUSTOMERS WHERE CUSTOMERID IS NULL;
SELECT CUSTOMERNAME FROM CUSTOMERS WHERE CITY IS NOT NULL;
```
* #### UPDATE CLAUSE
Used to update the DataBase or table
```
UPDATE table_name SET column1, column2 WHERE CustomerID is 10;
```

* #### DELETE CLAUSE
Used to delete the Database or table
```
DELETE FROM CUSTOMERS WHERE CUSTOMERID IS "1009";
DELETE FROM CUSTOMERS
```

* #### LIMIT CLAUSE
Used to display top N records from the database or table
```
SELECT * FROM CUSTOMERS LIMIT 5;
SELECT CUSTOMERID FROM CUSTOMERS WHERE CITY IS "London" LIMIT 5;
```

* ### SQL Functions
COUNT(): ```SELECT COUNT(*) FROM CUSTOMERS;``` \
SUM(): ```SELECT COUNT(*) FROM CUSTOMERS;```  \
AVG(): ```SELECT AVG(*) FROM CUSTOMERS;```  \
MIN(): ```SELECT MIN(CustomerID) FROM CUSTOMERS;```  \
MAX(): ```SELECT MAX(CustomerID) FROM CUSTOMERS;```

