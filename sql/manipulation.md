### [SQL](./README.md)
# Manipulation

Column Constraints

Column constraints are the rules applied to the values of individual columns:

    PRIMARY KEY constraint can be used to uniquely identify the row.
    UNIQUE columns have a different value for every row.
    NOT NULL columns must have a value.
    DEFAULT assigns a default value for the column when no value is specified.

There can be only one PRIMARY KEY column per table and multiple UNIQUE columns.

CREATE TABLE student (
  id INTEGER PRIMARY KEY,
  name TEXT UNIQUE,
  grade INTEGER NOT NULL,
  age INTEGER DEFAULT 10
);

CREATE TABLE Statement

The CREATE TABLE statement creates a new table in a database. It allows one to specify the name of the table and the name of each column in the table.

CREATE TABLE table_name (
  column1 datatype,
  column2 datatype,
  column3 datatype
);

INSERT Statement

The INSERT INTO statement is used to add a new record (row) to a table.

It has two forms as shown:

    Insert into columns in order.
    Insert into columns by name.

-- Insert into columns in order:
INSERT INTO table_name
VALUES (value1, value2);

-- Insert into columns by name:
INSERT INTO table_name (column1, column2)
VALUES (value1, value2);

ALTER TABLE Statement

The ALTER TABLE statement is used to modify the columns of an existing table. When combined with the ADD COLUMN clause, it is used to add a new column.

ALTER TABLE table_name
ADD column_name datatype;

DELETE Statement

The DELETE statement is used to delete records (rows) in a table. The WHERE clause specifies which record or records that should be deleted. If the WHERE clause is omitted, all records will be deleted.

DELETE FROM table_name
WHERE some_column = some_value;

UPDATE Statement

The UPDATE statement is used to edit records (rows) in a table. It includes a SET clause that indicates the column to edit and a WHERE clause for specifying the record(s).

UPDATE table_name
SET column1 = value1, column2 = value2
WHERE some_column = some_value;

