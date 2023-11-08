# EXP NO 2: DATA DEFINITION LANGUGE COMMANDS 
### DATE
## AIM:
To create a student database and execute DDL queries using SQL.


## THEORY
### DDL (Data Definition Language)

* DDL or Data Definition Language actually consists of the SQL commands that can be used to define the database schema.
* It simply deals with descriptions of the database schema and is used to create and modify the structure of database objects in the database.
* DDL is a set of SQL commands used to create, modify, and delete database structures but not data.
* These commands are normally not used by a general user, who should be accessing the database via an application.

 
### List of DDL commands: 
1. CREATE: This command is used to create the database or its objects (like table, index, function, views, store procedure, and triggers).
2. DROP: This command is used to delete objects from the database.
3. ALTER: This is used to alter the structure of the database.
4. TRUNCATE: This is used to remove all records from a table, including all spaces allocated for the records are removed.
5. RENAME: This is used to rename an object existing in the database.

## Query:
### 1) Create a database studentdb

### SQL QUERY:
```
Create database studentdb;
```
### OUTPUT:

![280675024-5968202e-2181-4492-9795-14088ac07bb7](https://github.com/prithviraj5703/DBMS/assets/121418418/ae722109-7256-4faa-82ff-c51cf451026c)



### 2) Create a table student with the following fieds RegisterNumber,Name,Age,Address,Phone number

### SQL QUERY: 
```
 create table student(rollno int,name char(20),age int,address varchar(20),phoneno int);
```

### OUTPUT:

![280675408-a475cc2c-991e-42d0-be06-760cd909cb7c](https://github.com/prithviraj5703/DBMS/assets/121418418/772e275b-c872-4236-96df-f755772e4c9a)



### 3) Alter the above student table by adding another attribute department

### SQL QUERY: 
```
alter table student add department char(30);
```

### OUTPUT:


![280676701-04623f48-4711-485a-9758-8251a8e292ed](https://github.com/prithviraj5703/DBMS/assets/121418418/89852206-d240-4ae9-8644-61b8fb7eb073)


### 4) Drop the student table
 
### SQL QUERY: 
```
drop table student;
```

### OUTPUT:



![280676966-0d1a229b-1a17-4a59-999d-89f6d9bf9d96](https://github.com/prithviraj5703/DBMS/assets/121418418/0f5e68f0-a94e-4182-9f1b-6c61f004bb1a)


### 5) Delete the student table using truncate keyword

### SQL QUERY: 
```
truncate table student;
```

### OUTPUT:


![280677263-a7ebfb1a-a69a-48c0-9aa3-76730edc2e5f](https://github.com/prithviraj5703/DBMS/assets/121418418/5438c887-1110-4381-af4c-23291086e5b4)



### 6) Rename the student table to mystudent

### SQL QUERY: 
```
alter table student rename to mystudent;
```


### OUTPUT:



![280677388-8586ae53-a448-4913-814e-ee695781ecfd](https://github.com/prithviraj5703/DBMS/assets/121418418/56f77a07-f4a0-4a20-af6a-6b1ff218edb5)


## Result:
         Thus the basic DDL commands in SQL are executed. 


