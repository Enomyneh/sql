# SQL Statements

## Create

```sql
CREATE TABLE IF NOT EXISTS table_a
  column 
    INTEGER
    BOOLEAN
    FLOAT
    VARCHAR()
    TEXT
    DATE
    DATETIME
      PRIMARY KEY
      AUTOINCREMENT
      UNIQUE
      NOT NULL
        DEFAULT

```

## Alter

```sql
ALTER TABLE table_a
ADD column
DROP column
RENAME TO table_b
```

## Drop

```sql
DROP TABLE IF EXISTS table_a
```

### Select

```sql
SELECT/SELECT DISTINCT column, *
  COUNT(*),
  COUNT(column)
  MIN(column)
  MAX(column)
  AVG(column)
  SUM(column)
FROM table_name
JOIN/INNER JOIN 
LEFT JOIN
RIGHT JOIN
FULL JOIN table_b
  ON table_a.id = table_b.id
WHERE condition
  AND
  OR
	  =
	  !=
	  LIKE
	  NOT LIKE
	  IN ()
	  NOT IN ()
	  %
	  _
	  IS NULL
	  IS NOT NULL
GROUP BY column
HAVING constraint
ORDER BY column
  ASC
  DESC
LIMIT count
OFFSET count
```

## Insert

```sql
INSERT INTO table
  (column_a, columnb_b)
VALUES 
  (value_1, value_2)
```

## Update

```sql
UPDATE table
SET column_a = value_1
    column_b = value_2
WHERE condition
```

## Delete

```sql
DELETE FROM table
WHERE condition
```
