## Database and Table Manipulation


**Create a database:**
```sql
CREATE DATABASE database_name
```


**Delete a database:**
```sql
DROP DATABASE database_name
```


**Create a table in a database:**
```sql
CREATE TABLE table_name ("col1" "col1_data_type", "col2" "col2_data_type",..)
```


**Add columns in an existing table:**
```sql
ALTER TABLE table_name ADD col_name col_type
```


**Delete columns in an existing table:**
```sql
ALTER TABLE table_name DROP col_nam col_type
```


**Delete a table:**
```sql
DROP TABLE table_name
```

---------------------------------------------------

## Insert, Update & Delete:

**Insert new rows into a table:**
```sql
INSERT INTO table_name 
VALUES (value1, value2, ....)
```


Update one or several columns in rows
```sql
UPDATE  table_name 
   SET  col_name_1=new_value_1, 
        col_name_2= new_value2
  WHERE
        col_name=some_value


Delete rows in a table
    • DELETE FROM table_name 
WHERE 
column_name=somevalue



           Select

Select data from a table
    • SELECT column(s) FROM table_name

Select all data from a table
    • SELECT * FROM table_name


Select only distinct (different) data from a table
    • SELECT DISTINCT col_name FROM table_name


Select only certain data from a table
    • SELECT col_name(s) FROM table_name
WHERE 
col operator value AND column
operator value OR column
operator value AND (..OR..)

IN operator (exact value needed to return)
    • SELECT col names table_name 
WHERE column_name
IN (value1, value2...)

Select data from a table with sort the rows
    • SELECT column names FROM table_name
ORDER BY row_1,
row_2 DESC,
row_3 ASC

Group By
    • SELECT column_1, ..,
SUM (group_column_name)
FROM table_name GROUP BY
group_column_name

Select data from table(S) and insert it into another
    • SELECT column_name(s) 
INTO new_table FROM source_table_name
WHERE query
