# Scraping all products from Tiki
**Phuong T.M. CHU**

**Scraping all products from Tiki** is the project that I finished after the first week of studying Machine Learning.

## Introduction

PostgreSQL is a free and open-source relational database management system. Using a database instead of regular spreadsheet will allow us to store a larger amount of data as well as offer a much higher capacity to later process our data. 

**In this project, we push the data of all [Tiki](https://tiki.vn/) products to a PostgreSQL database.** 

## PostgreSQL
### Connect to PostgreSQL database server

Here below is a list of common `psql` commands that helps you work with PostgreSQL.

### Connect to PostgreSQL database

The following command connects to a database under a specific user. After pressing Enter PostgreSQL will ask for the password of the user.

`psql -d dbname -U  username -W`

If you want to connect to a database that resides on another host, you add the -h option as follows:

`psql -h host -d database -U user -W`

### Get help on psql commands

To know all available psql commands, you use

`\?`

To get help on specific PostgreSQL statement, you use (for example)

`h ALTER TABLE`

### Switch connection to a new database

Once you are connected to a database, you can switch the connection to a new database

`\c dbname username`

### List available databases

To list all databases in the current PostgreSQL database server, you use

`\l`

### List available tables

To list all tables in the current database, you use

`\dt`

### Describe a table

To describe a table such as a column, type, modifiers of columns, etc., you use

`\d tablename`

### List users and their roles

To list all users and their assign roles, you use

`\du`

### Turn on query execution time

To turn on query execution time, you use

`\timing`

You use the same command `\timing` to turn it off.

### Edit command in your own editor

It is very handy if you can type the command in your favorite editor. To do this in psql, you use

`\e`

### Switch output options

`psql` supports some types of output format and allows you to customize how the output is formatted on the fly.

* `\a` command switches from aligned to non-aligned column output.
* `\H` command formats the output to HTML format.

### Quit psql

To quit psql, you use

`\q`

### Creating tables

### Connecting to Postgres from Python

In Python, there is an open source library called [psycopg2](http://initd.org/psycopg/) that implements the Postgres protocol to connect to our Postgres server. You can think of psycopg2 being similar to connecting to a SQLite database using the [sqlite3](https://docs.python.org/3.5/library/sqlite3.html) library.
