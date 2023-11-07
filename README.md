# Date:
# Aim
To create a student database and execute DDL queries using SQL.


## DDL (Data Definition Language)
<div align="justify">
DDL or Data Definition Language actually consists of the SQL commands that can be used to define the database schema. It simply deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database. DDL is a set of SQL commands used to create, modify, and delete database structures but not data. These commands are normally not used by a general user, who should be accessing the database via an application.

List of DDL commands: 
</div>

## List of DDL commands: 

<div align="justify">
CREATE: This command is used to create the database or its objects (like table, index, function, views, store procedure, and triggers).
DROP: This command is used to delete objects from the database.
ALTER: This is used to alter the structure of the database.
TRUNCATE: This is used to remove all records from a table, including all spaces allocated for the records are removed.
RENAME: This is used to rename an object existing in the database.

</div>

## Query:
### 1) Create a table student with the following fieds rollno,name,age,address,phoneno.
### SQL QUERY: 
```sql
CREATE TABLE Student (
		roll_no NUMERIC,
        std_name VARCHAR(10),
        std_age NUMERIC,
        address VARCHAR(50),
        phno NUMERIC
        );
	INSERT INTO Student(roll_no, std_name, std_age, address, phno) VALUES (121,'Prakash',19,'Leo nagar,Tambaram,Chennai',987654321);
	INSERT INTO Student(roll_no, std_name, std_age, address, phno) VALUES (122,'Aakash',19,'SVM,Perambur,Chennai',9677202658);
	INSERT INTO Student(roll_no, std_name, std_age, address, phno) VALUES (123,'Vikash',18,'Raja nagar,Hosur,Krishnagiri',987654321);
  SELECT *FROM Student;
```

### OUTPUT:
![Screenshot 2023-09-28 125335](https://github.com/Sabariakash22009103/G2_DBMS/assets/119390227/f4bab3f8-b730-4c74-8bb0-c0fce2876e28)

### 2) Change the above student table by adding another attribute department
### SQL QUERY: 
```sql
ALTER TABLE Student ADD dept VARCHAR(30);
INSERT INTO Student(roll_no, std_name, std_age, address, phno,dept) VALUES (121,'Prakash',19,'Leo nagar,Tambaram,Chennai',987654321,'CSE');
INSERT INTO Student(roll_no, std_name, std_age, address, phno,dept) VALUES (122,'Aakash',19,'SVM,Perambur,Chennai',9677202658,'AI&DS');
INSERT INTO Student(roll_no, std_name, std_age, address, phno,dept) VALUES (123,'Vikash',18,'Raja nagar,Hosur,Krishnagiri',987654321,'ECE');
SELECT *FROM Student;
```
### OUTPUT:
![Screenshot 2023-09-28 131911](https://github.com/Sabariakash22009103/G2_DBMS/assets/119390227/d0a47ae4-6b9e-4e9d-947d-7fbd8d07f06b)

### 3) Drop the student table
### SQL QUERY: 
```sql
DROP TABLE Student;
SELECT *FROM Student;
```
### OUTPUT:
![Screenshot 2023-09-28 133840](https://github.com/Sabariakash22009103/G2_DBMS/assets/119390227/2f9fb89a-4085-4e3d-b28b-3b665ef4e087)

### 4) Delete the student table using truncate keyword
### SQL QUERY:
```sql
TURNCATE TABLE Student;
SELECT *FROM Student;
```
### OUTPUT:
![image](https://github.com/Sabariakash22009103/G2_DBMS/assets/119390227/c21ba4e1-3c1d-4cc0-898e-ddf2deb80b0e)

### 5) Rename the student table to mystudent

### SQL QUERY: 
```sql
ALTER TABLE Student RENAME TO Mystudent;
SELECT *FROM Mystudent;
```
### OUTPUT:
![Screenshot 2023-09-28 125335](https://github.com/Sabariakash22009103/G2_DBMS/assets/119390227/f4bab3f8-b730-4c74-8bb0-c0fce2876e28)
### RESULT:
To create a student database and execute DDL queries using SQL is executed successfully.
