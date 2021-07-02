# Oracle-SQL
SQL query and solutions

Table of Contents
Finding Data Queries.
Data Modification Queries.
Altering Table Queries.
Creating Table Query.

1. Finding Data Queries
SELECT: used to select data from a database
SELECT * FROM table_name;

DISTINCT: filters away duplicate values and returns rows of specified column
SELECT DISTINCT column_name;

WHERE: used to filter records/rows
SELECT column1, column2 FROM table_name WHERE condition;
SELECT * FROM table_name WHERE condition1 AND condition2;
SELECT * FROM table_name WHERE condition1 OR condition2;
SELECT * FROM table_name WHERE NOT condition;
SELECT * FROM table_name WHERE condition1 AND (condition2 OR condition3);


LIKE: operator used in a WHERE clause to search for a specific pattern in a column
% (percent sign) is a wildcard character that represents zero, one, or multiple characters
_ (underscore) is a wildcard character that represents a single character
SELECT column_names FROM table_name WHERE column_name LIKE pattern;
LIKE ‘a%’ (find any values that start with “a”)
LIKE ‘%a’ (find any values that end with “a”)
LIKE ‘%or%’ (find any values that have “or” in any position)
LIKE ‘_r%’ (find any values that have “r” in the second position)
LIKE ‘a_%_%’ (find any values that start with “a” and are at least 3 characters in length)
LIKE ‘[a-c]%’ (find any values starting with “a”, “b”, or “c”



2. Data Modification Queries
INSERT INTO: used to insert new records/rows in a table
INSERT INTO table_name (column1, column2) VALUES (value1, value2);
INSERT INTO table_name VALUES (value1, value2 …);
UPDATE: used to modify the existing records in a table
UPDATE table_name SET column1 = value1, column2 = value2 WHERE condition;
UPDATE table_name SET column_name = value;
DELETE: used to delete existing records/rows in a table
DELETE FROM table_name WHERE condition;
DELETE * FROM table_name;


3. View Queries
CREATE: create a view
CREATE VIEW view_name AS SELECT column1, column2 FROM table_name WHERE condition;
SELECT: retrieve a view
SELECT * FROM view_name;
DROP: drop a view
DROP VIEW view_name;

4. Altering Table Queries
ADD: add a column
ALTER TABLE table_name ADD column_name column_definition;
MODIFY: change data type of column
ALTER TABLE table_name MODIFY column_name column_type;
DROP: delete a column
ALTER TABLE table_name DROP COLUMN column_name;

5. Creating Table Query
CREATE: create a table
CREATE TABLE table_name (
column1 datatype,
column2 datatype,
column3 datatype,
column4 datatype,
);
