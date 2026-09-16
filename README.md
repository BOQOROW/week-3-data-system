mysql> USE sales;
Database changed
mysql> CREATE TABLE student (
    ->     id INT PRIMARY KEY,
    ->     fullName VARCHAR(100),
    ->     age INT
    -> );
Query OK, 0 rows affected (0.15 sec)

mysql> INSERT INTO student (id, fullName, age)
    -> VALUES
    ->     (1, 'Alice Johnson', 19),
    ->     (2, 'Bob Smith', 18),
    ->     (3, 'Charlie Brown', 21);
Query OK, 3 rows affected (0.04 sec)
Records: 3  Duplicates: 0  Warnings: 0

mysql> UPDATE student
    -> SET age = 20
    -> WHERE id = 2;
Query OK, 1 row affected (0.01 sec)
Rows matched: 1  Changed: 1  Warnings: 0
