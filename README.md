# DataBase

# Employee DBMS

This repository contains a SQL script to manage an employee database. The database includes basic operations such as adding, updating, retrieving, and deleting employee records.



## Database Schema

```sql
CREATE TABLE "Employ" (
	"id"	INTEGER,
	"name"	TEXT,
	"salery"	INTEGER,
	"phone"	INTEGER,
	PRIMARY KEY("id" AUTOINCREMENT)
);
```

## 1. Adding Employees (Create)

### Add a New Employee

```sql
INSERT INTO Employ(name,phone,salery,role)
VALUES('Mehul',011255553,25000,'CEO');
```

### Add Multiple Employees

```sql
INSERT INTO Employ(name,phone,salery,role)
VALUES('Mehul',011255553,25000,'CEO'),
('Darshan Patel',011255553,125000,'faunder');
```

## 2. Retrieving Employee Information (Read)

### All Employee Information

```sql
SELECT*FROM Employ;
```

### Specific Columns for All Employees

```sql
SELECT name,salery FROM Employ;
```

### Employees with a Specific Role

```sql
SELECT * FROM Employ WHERE role='CEO';SELECT * FROM Employ WHERE role='CEO';
```



### Employees Older than 30 and Earning More than $70,000

```sql
SELECT * FROM Employ WHERE salery >20000;
```

## 3. Updating Employee Information (Update)

### Change Salary

```sql
UPDATE Employ SET salery = 1500 WHERE id=4;
```



## 4. Deleting Employees (Delete)

### Remove an Employee by ID

```sql
DELETE FROM Employ WHERE id=1;
```

### Delete Employees by Age

```sql
DELETE FROM employees WHERE age < 18;
```
