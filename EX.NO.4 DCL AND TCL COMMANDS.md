# EX.NO 4 Data Control Language (DCL) Commands and Transaction Control Languages (TCL) in SQL
### DATE:
## AIM:
To create a manager database and execute DML queries using SQL.
```
DEVELOPED BY:Mohanish.K
REG NO: 22002294
```
# THEORY
## Data Control Language (DCL) commands
* Data control language (DCL) is used to access the stored data.
* It is mainly used for revoke and to grant the user the required access to a database.
## List of DCL commands: 
1. GRANT : It is used to insert data into a table.
2. REVOKE: It is used to update existing data within a table.
## Transaction control language(TCL) commands
1. COMMIT : COMMIT command in SQL is used to save all the transaction-related changes permanently to the disk
2. START TRANSACTION : to start the transaction
3. ROLLBACK : undo the transaction upto savepoint 
4. SAVEPOINT : create a savepoint to save the different parts of the same transaction using different names

### Q1) Create a table employee with employee id ,name and Address

### QUERY:
```
sql create table employee( emp_id numeric, emp_name varchar(10), addr varchar(40) );
```
### OUTPUT:


![276302151-56bbda44-a582-42e3-9738-5b1d035dd675](https://github.com/prithviraj5703/DBMS/assets/121418418/908d4d45-29fd-4bfc-8cdc-dd428fb7afec)



### Q2) Insert three rows into emploee table 


### QUERY:
```
insert into employee values(1,'Luffy','EastBlue');
insert into employee values(2,'Shanks','GodValley');
insert into employee values(3,'Grap','MarinFord');
```

### OUTPUT:


![276302974-db081e71-759d-44df-b847-75294a2e2a34](https://github.com/prithviraj5703/DBMS/assets/121418418/1315e7df-0d1c-46de-948b-dfe79e765239)




### Q3) Start the transaction and create a save point s1.

### QUERY:
```
savepoint A;
```

### OUTPUT:


![276303398-d491985f-d652-4510-baba-69bda39920c4](https://github.com/prithviraj5703/DBMS/assets/121418418/8e4396ca-e6a5-4720-a145-41ee98967b98)




### Q4) Perform insertion into employee table.

### QUERY:
```
insert into employee(4,'Robin','EniesLobby');
```

### OUTPUT:


![276303961-b9d81949-f840-4fb4-8427-6c5efb79da74](https://github.com/prithviraj5703/DBMS/assets/121418418/a13a45ea-5cc2-4287-b393-c9e0e93e6528)




### Q5)	Display the employee table and create a save point s2 .


### QUERY:
```
select * from employee;
savepoint s2;
```

### OUTPUT:



![276304509-bc86bb69-d7ad-4193-aeda-050214882984](https://github.com/prithviraj5703/DBMS/assets/121418418/69203db1-473c-44bd-bdaa-67445883c704)




### Q6)	Perform updation on any one of the row.


### QUERY:
```
update employee set emp_name='Nico Robin' where emp_id=4;
```

### OUTPUT:


![276305358-2e9e6855-56ea-40f4-ba36-56f8eafd68ee](https://github.com/prithviraj5703/DBMS/assets/121418418/c0f1603b-725d-4c84-828b-2d20d1ee3bac)





### Q7) Display the employee table and rollback to  save point s2 


### QUERY:
```
select * from employee;
rollback to s2;
```






### OUTPUT:



![276305855-b66b2852-7cbc-49e6-a059-579485f3ff49](https://github.com/prithviraj5703/DBMS/assets/121418418/7831ab0c-d366-4b3f-9adf-ef1aaf17a553)








### Q8) Display the employee table and commit the changes; 


### QUERY:
```
select * from employee;
commit;
```

### OUTPUT:



![276306207-7dd55645-f515-4c5b-9174-1b3a9bc24e30](https://github.com/prithviraj5703/DBMS/assets/121418418/c089fd0e-c30b-413b-9900-8fe37345e25c)





### Q9) Rollback to save point s1;


### QUERY:
```
rollback to A;
```

### OUTPUT:



![276306832-441afff5-9f95-418b-ad8b-c2b5cfbf810d](https://github.com/prithviraj5703/DBMS/assets/121418418/861b155e-7c26-4e52-aa65-29030b00c7dd)




## RESULT :
Thus the basic TCL and DCL commands are executed.
