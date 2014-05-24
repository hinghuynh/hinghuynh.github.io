---
layout: post
title: SQL Injections
date: May 17, 2014
category: code
customid: week7technical
---
SQL injection is the use of code to exploit security vulnerabilities of SQL databases to manipulate or exploit the data that lies within the database. Successful malicious attempts of SQL injections can read sensitive data from the database, modifying database data using SQL commands like insert, update, or delete, as well as execute administration operations on the database. With these SQL injections, attackers can spoof identity or tamper with existing data such as voiding transaction or changing balances, disclosure all data on the system, or blatantly destroying all the data.

Here are some simple SQL statements that have been used as implemented in the past.

```
' or '1'='1' -- ' or '1'='1' ({ ' or '1'='1' /*
````
Here are some simple SQL statements that have been used as implemented in the past.

```
SELECT * FROM users WHERE name = '' OR '1'='1'; 
SELECT * FROM users WHERE name = '' OR '1'='1' -- ';
```
This statement would always render true, allowing possible spoof of identity in a user login input field. 
Another simple SQL command is

```
';DROP TABLE users; SELECT * FROM userinfo WHERE 't' = 't
```
If this SQL injection was successful you could completely delete a database. 

One of the things you can do to prevent SQL injections from occurring with against your databases is to use prepared statements and parameterized queries. These are SQL statements that sent and parse by the database server separate from any parameters. This allows you separate your actual SQL separate from the parameters. Any parameters you send when using the prepared statement would be separated into a string so that the search would search the entire string for the parameter input. 

For example, notice that the follow user input is an entire string when sent with a prepared statement. 

```
'Sarah'; DELETE FROM employees 
SELECT * FROM users WHERE name = "'Sarah'; DELETE FROM employees";
```
