# SQL Queries 
## `SELECT` Query in SQL
The SELECT statement is used to retrieve data from a database. It's one of the most commonly used SQL commands.
### Basic Syntax
```bash
    SELECT column1, column2
    FROM table_name;
```
- **`column1, column2, ...`:** The columns you want to retrieve from the table.
- **`table_name` :**The name of the table from which to retrieve data.
### Selecting All Columns
To select all columns from a table, use the **`*`** wildcard.
```bash
    SELECT * 
    FROM employees;
```
### Selecting Specific Columns
If you want to retrieve only specific columns, list them
```bash
    SELECT first_name, last_name 
    FROM employees;
```
### Using WHERE Clause
You can filter the results by specifying conditions using the **`WHERE`** clause:
```bash
    SELECT first_name, last_name 
    FROM employees 
    WHERE department = 'Sales';
```
This retrieves the **`first_name`** and **`last_name`** of **employees** in the "**Sales**" department.
### Sorting the Results
To order the results, use the **`ORDER BY`** clause.
```bash
    SELECT first_name, last_name 
    FROM employees 
    ORDER BY last_name ASC;
```
This retrieves the **`first_name`** and **`last_name`** columns and sorts the results by **last_name** in **Ascending Order**.