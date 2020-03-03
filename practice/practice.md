# Unit 7, Lesson 5

## Introduction to Databases & SQL

### Practice

**Exercise 0- DATABASES:**
**What are relational vs. non-relational databases?**

**Exercise 1: SET UP**
Visit the [postgres.app](https://postgresapp.com/). Follow the instructions to install PostgreSQL and the command line tools.
Ensure that you complete all steps for Downloading, Initializing, and Configuring.

Download [Postico](https://eggerapps.at/postico/) or another graphical user interface (GUI) where you can ultimately write SQL queries. Postico is free! Follow the instructions on the website for set up.

OPTIONAL: If you are more of a visual learner, set up Postgres and a GUI as you follow along with this [Installing PostgreSQL Video](https://www.youtube.com/watch?v=xaWlS9HtWYw).

**Exercise 2: ACCESS COMMAND LINE**
Go to the command line and connect to your database by running the command `psql`. Now you are connected to PostgreSQL. To exit from PostgreSQL, use `control d`.

Run the command `\l` within your `psql` command line.
**What is does the `l` command output?**

**Exercise 3: CREATE DATABASE AND CONNECT**
Create a database called `marcy` by running the command `create database marcy;` **NOTE** the semi-colon is important! Makes sure to include it. You have successfully created a database if your `psql` command line outputs `CREATE DATABASE`.

Next, connect to your database by running the command `\c`. Successfully connecting to your database will output `You are now connected to database "marcy" as user "[your username]"`.

**Exercise 4: CREATE TABLES**
Created a table called `projects` by running the command
`create table projects(id SERIAL PRIMARY KEY, name TEXT NOT NULL, partners TEXT NOT NULL);`

**Based on this command, what do you imagine the rows and columns of your projects table to be?**

To see a description of the table you just created, run the command `\d lessons`.

**Exercise 5: BASIC QUERIES - POPULATE TABLES**
Give your table some data. Follow the Postgres documentation for [populating tables with rows](https://www.postgresql.org/docs/12/tutorial-populate.html).

Run the command `INSERT INTO lessons VALUES(1, 'data structures', 'ruben');`

Input 5 more lessons using the same syntax for different lessons and partners.

**Exercise 6: BASIC QUERIES - SELECT DATA**
Run the command `SELECT * FROM lessons`. **What does this command do?**

Run other SELECT commands and use the [Querying a Table Documentation as a reference](https://www.postgresql.org/docs/12/tutorial-select.html)

**Write a reflection on the pros and cons of inputting and accessing data using the `INSERT` and `SELECT` commands.**

**Exercise 7: MORE BASIC QUERIES**
PostgreSQL Exercises Provides listings of simple SQL Queries.
Keep your documentation handy.
Visit the [exercises](https://pgexercises.com/questions/basic/).
Solutions are embedded in the exercise app.