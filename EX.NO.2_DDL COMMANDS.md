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

![280675024-5968202e-2181-4492-9795-14088ac07bb7](https://github.com/DrUmaRaniV/DBMS/assets/121418418/efc74325-d663-435e-b61d-334c80f6a764)


### 2) Create a table student  and insert any two rows with the following fieds RegisterNumber,Name,Age,Address,Phone number

### SQL QUERY: 
```
 create table student(rollno int,name char(20),age int,address varchar(20),phoneno int);
```

### OUTPUT:

![280675408-a475cc2c-991e-42d0-be06-760cd909cb7c](https://github.com/DrUmaRaniV/DBMS/assets/121418418/2afd3bb6-f00c-4631-927f-bd012eb470a4)


### 3) Alter the above student table by adding another attribute department

### SQL QUERY: 
```
alter table student add department char(30);
```
### OUTPUT:

![280676701-04623f48-4711-485a-9758-8251a8e292ed](https://github.com/DrUmaRaniV/DBMS/assets/121418418/d5722176-cb11-42bd-a59c-21892ffeed20)



### 4) Rename the student table to mystudent

### SQL QUERY: 
```
drop table student;
```


### OUTPUT:


![280676966-0d1a229b-1a17-4a59-999d-89f6d9bf9d96](https://github.com/DrUmaRaniV/DBMS/assets/121418418/fddcc107-953e-4090-a796-f3ae45cdbda5)



### 5) Delete the mystudent rows using truncate keyword

### SQL QUERY: 
```
truncate table student;
```

### OUTPUT:

![280677263-a7ebfb1a-a69a-48c0-9aa3-76730edc2e5f](https://github.com/DrUmaRaniV/DBMS/assets/121418418/a68c45b0-4f96-495a-9f42-91be2699d3c7)


### 6) Drop the mystudent table
 
### SQL QUERY: 
```
alter table student rename to mystudent;
```

### OUTPUT:




![280677388-8586ae53-a448-4913-814e-ee695781ecfd](https://github.com/DrUmaRaniV/DBMS/assets/121418418/dc17ec00-322d-48ac-8fd0-31081116471e)





## Result:
         Thus the basic DDL commands in SQL are executed. 


