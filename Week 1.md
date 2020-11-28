# Week 1

## Basic SQL

### CREATE table

```sql
CREATE TABLE table_name
	(
        column_name_1 datatype optional_parameters,
        column_name_2 datatype,
        ...
        column_name_n datatype
	)
```

Ex: Create a table for Canadian provinces

```sql
CREATE TABLE provinces(
	id char(2) PRIMARY KEY NOT NULL,
    name varchar(24)
	)
```

| id<br />*char(2)* | name<br />*varchar(24)* |
| ----------------- | ----------------------- |
| AB                | ALBERTA                 |
| BC                | BRITISH COLUMBIA        |
| ...               | ...                     |

Ex: 

```sql
CREATE TABLE author (
	author_id CHAR(2) PRIMARY KEY NOT NULL,
    lastname VARCHAR(15) NOT NULL,
    firstname VARCHAR(15) NOT NULL,
    email VARCHAR(40),
    cith VARCHAR(15),
    country CHAR(15)
)
```



VARCHAR: variable length

CHAR: fixed length



Ex:

```sql
drop table COUNTRY; 
create table COUNTRY (
	ID int NOT NULL,
    CCODE char(2),
    NAME varchat(60),
    PRIMARY KEY (ID)
)
```



### SELECT Statement

```sql
Select statement: Query
Result from the query: Result set/table

Select * from <tablename>		#selete all columns
select column 1, column 2, column 3, ..., column n from tablename
	WHERE column n =/>/</>=/<=/<> xxxx

```

Ex:

```sql
select book_id, title from Book
	WHERE book_id = 'B1'
```

