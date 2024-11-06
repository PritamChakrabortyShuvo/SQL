# SQL (Structured Query Language)
SQL is a standard programming language used to manage and manipulate relational databases. It allows us to create, read, update & delete data in a database.

With SQL, we can :
- **Query Data :** Retrieve specific information from the database.
- **Insert Data :** Add new records to tables.
- **Update Data :** Modify existing records.
- **Delete Data :** Remove records.
- **Define Structure :** Create and modify tables and database schema.

SQL is widely used in relational database systems like MySQL, PostgreSQL, Oracle & SQL Server. Making it essential for working with structured data in relational databases.
## Tables in SQL
In SQL, a table is where data is stored in a structured format. It's made up of rows and columns and forms the fundamental unit of storage in a relational database.
## Key Components of a Table:
Table names should 
- Be lowercase.
- Have no spaces—use underscores instead.
- Refer to a collective group or be plural.
### Columns
A field is a column that holds one piece of information about all records.
- Tables columns are refered as Fields.
- Each column holds a specific type of data (e.g., integers, strings, dates).
- Each column has a name and a data type (e.g., INT, VARCHAR, DATE).
- Columns are set at database creation.
- Field names should :
    - Be lowercase.
    - Have no spaces.
    - Be singular.
    - Be different from other field names.
    - Be different from the table name.
### Rows
A record is a row that holds data on an individual observation.
- Table rows are referred as records.
- Each row represents a single record in the table.
- There is no limit to the number of records.
### Primary Key
Unique identifiers are used to identify records in a table. They are unique and often numbers.
- A unique identifier for each row, ensuring that no two rows have the same value for this column.
- **Example :** An "id" column with unique values for each row.
### Foreign Key
- A column in one table that refers to the primary key of another table, establishing a relationship between the two.
- **Example :** A "department_id" in the "employees" table might be a foreign key referring to the "id" in the "departments" table.
### Constraints
Constraints are rules applied to table columns to enforce data integrity. 
- **Example :** NOT NULL, UNIQUE, CHECK, etc.