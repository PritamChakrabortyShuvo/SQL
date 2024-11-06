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
## Key Components of a Table
Table names should 
- Be lowercase.
- Have no spaces—use underscores instead.
- Refer to a collective group or be plural.
<div align="center">
    <img src="Diagram" width=30%>
</div>

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
## SQL Data Types
In SQL, data types define the type of data that can be stored in a column of a table. Each column must be assigned a data type when the table is created & it determines the kind of values the column can store.
## Common SQL Data Types
### Numeric Types
- **INT :** Used to store integers (whole numbers).
    - **Example :** **`age INT`**
- **DECIMAL** or **NUMERIC :** Used to store exact numeric values with a specified precision and scale.
    - **Example :** **`price DECIMAL(10, 2)`** (10 total digits, 2 digits after the decimal point).
- **FLOAT / REAL :** Used for approximate numeric values, typically with floating-point precision.
    - **Example :** **`height FLOAT`**
<div align="center">
    <img src="Diagram" width=30%>
</div>

### Character/String Types
- **CHAR(n) :** Fixed-length character string. If the data is shorter than n, it will be padded with spaces.
    - **Example :** **`gender CHAR(1)`**
- **VARCHAR(n) :** Variable-length character string. Can store strings up to **`n`** characters.
    - **Example :** **`name VARCHAR(100)`**
- **TEXT :** Used for storing large text values.
    **Example :** **`description TEXT`**
<div align="center">
    <img src="Diagram" width=30%>
</div>

### Date and Time Types
- **DATE :** Stores date values (year, month, day).
    - **Example :** **`birth_date DATE`**
- **TIME :** Stores time values (hour, minute, second).
    - **Example :** **`start_time TIME`**
- **DATETIME :** Stores both date and time values.
    - **Example :** **`created_at DATETIME`**
- **TIMESTAMP :** Similar to DATETIME but typically used for tracking changes and storing the time of an event in a database.
    - **Example :** **`last_updated TIMESTAMP`**
<div align="center">
    <img src="Diagram" width=30%>
</div>

### Boolean Type
- **BOOLEAN :** Stores TRUE or FALSE values.
    - **Example :** is_active BOOLEAN
### Binary Types
- **BLOB (Binary Large Object) :** Used to store binary data such as images, audio or other files.
    - **Example :** **`profile_picture BLOB`**
### Other Data Types
- **ENUM :** A string object with a predefined list of values (useful for columns that have a fixed set of options).
    - **Example :** **`status ENUM('active', 'inactive', 'suspended')`**
- **JSON :** Stores JSON formatted data for structured but flexible storage.
    - **Example :** **`preferences JSON`**