# My_Sql

1. What is MySQL?

MySQL is a database management system for web servers. It can grow with the website as it is highly scalable. Most of the websites today are powered by MySQL.

2. What are some of the advantages of using MySQL?

Flexibility: MySQL runs on all operating systems
Power: MySQL focuses on performance
Enterprise-Level SQL Features: MySQL had for some time been lacking in advanced features such as subqueries, views, and stored procedures.
Full-Text Indexing and Searching
Query Caching: This helps enhance the speed of MySQL greatly
Replication: One MySQL server can be duplicated on another, providing numerous advantages
Configuration and Security

3. What do you mean by ‘databases’?

A database is a structured collection of data stored in a computer system and organized in a way to be quickly searched. With databases, information can be rapidly retrieved.

4. What does SQL in MySQL stand for?

The SQL in MySQL stands for Structured Query Language. This language is also used in other databases such as Oracle and Microsoft SQL Server.  One can use commands such as the following to send requests from a database:

SELECT title FROM publications WHERE author = ' J. K. Rowling’;

Note that SQL is not case sensitive. However, it is a good practice to write the SQL keywords in CAPS and other names and variables in a small case.

5. What does a MySQL database contain?

A MySQL database contains one or more tables, each of which contains records or rows. Within these rows are various columns or fields that contain the data itself.

6. How can you interact with MySQL?

There are three main ways you can interact with MySQL: 

using a command line
via a web interface
through a programming language

7. What are MySQL Database Queries?

A query is a specific request or a question. One can query a database for specific information and have a record returned.

8. What are some of the common MySQL commands?

![Screenshot (987)](https://user-images.githubusercontent.com/81725794/184502320-6e6460f3-57cb-43a1-95ff-15158f5e71fe.png)

![Screenshot (988)](https://user-images.githubusercontent.com/81725794/184502324-a7396f0e-41b9-41e1-8d1e-a45b79444486.png)

9. How do you create a database in MySQL?

Use the following command to create a new database called ‘books’:

CREATE DATABASE books;

10. How do you create a table using MySQL?

Use the following to create a table using MySQL:

CREATE TABLE history (
author VARCHAR(128),
title VARCHAR(128),
type VARCHAR(16),
year CHAR(4)) ENGINE InnoDB;

11. How do you Insert Data Into MySQL?

The INSERT INTO statement is used to add new records to a MySQL table:

INSERT INTO table_name (column1, column2, column3,...)
VALUES (value1, value2, value3,...)
If we want to add values for all the columns of the table, we do not need to specify the column names in the SQL query. However, the order of the values should be in the same order as the columns in the table. The INSERT INTO syntax would be as follows:

INSERT INTO table_name
VALUES (value1, value2, value3, ...);

12. How do you remove a column from a database?

You can remove a column by using the DROP keyword:

ALTER TABLE classics DROP pages;

13. How to create an Index in MySQL?

In MySQL, there are different index types, such as a regular INDEX, a PRIMARY KEY, or a FULLTEXT index. You can achieve fast searches with the help of an index. Indexes speed up performance by either ordering the data on disk so it's quicker to find your result or, telling the SQL engine where to go to find your data.

Example: Adding indexes to the history table:

ALTER TABLE history ADD INDEX(author(10));
ALTER TABLE history ADD INDEX(title(10));
ALTER TABLE history ADD INDEX(category(5));
ALTER TABLE history ADD INDEX(year);
DESCRIBE history;

14. How to Delete Data From a MySQL Table?

In MySQL, the DELETE statement is used to delete records from a table:

DELETE FROM table_name
WHERE column_name = value_name

15. How do you view a database in MySQL?
