# Ex. No: 7 PL/SQL program -BIGGEST OF THREE NUMBERS  
### DATE: 
### AIM: To create PL/SQL program to find biggest of three numbers.

### ALGORITHM:
1. Declare the variable a, b, c and assign value in Declare section.
2. begin the section
3. Find biggest of three numbers 
4. 5. Display the result 
6. End the begin section.

### Program:
```
DEVELOPED BY:V.PRITHVIRAJ
REG NO: 212222100038
```
```

DECLARE
  
  num1 NUMBER := 10; 
  num2 NUMBER := 20; 
  num3 NUMBER := 15;
  biggest NUMBER;
BEGIN
  
  IF num1 >= num2 AND num1 >= num3 THEN
    biggest := num1;
  ELSIF num2 >= num1 AND num2 >= num3 THEN
    biggest := num2;
  ELSE
    biggest := num3;
  END IF;


  DBMS_OUTPUT.PUT_LINE('The biggest number is: ' || biggest);
END;
/
```
### Output:




![276867083-c45bc1ec-23a9-4554-9b19-91b8a9ce15d2](https://github.com/prithviraj5703/DBMS/assets/121418418/cafbf289-9ac7-4410-8104-4b14b9f84c33)



### Result:
Thust the program was performed sucessfully.
