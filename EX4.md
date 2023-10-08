# Ex. No: 4 Creating Procedures using PL/SQL

### AIM: To create a procedure using PL/SQL.

### Steps:
1. Create employee table with following attributes (empid NUMBER, empname VARCHAR(10), dept VARCHAR(10),salary NUMBER);
2. Create a procedure named as insert_employee data.
3. Inside the procdure block, write the query for inserting the values into the employee table.
4. End the procedure.
5. Call the insert_employee data procedure to insert the values into the employee table.
6. Display the employee table

### Program:
```

NAME: R KAVI KEERTHANA
Reg.no:  212222100022

```
```
 create table empl(empid number,empname varchar (20), dept varchar (10) ,salary number);

Table created.

SQL> create or replace procedure insert_empl_data AS
  2  begin
  3  insert into empl (empid,empname,dept,salary)
  4  values (1,'kavi','MD',5000000);
  5  insert into empl (empid,empname,dept,salary)
  6  values (2,'mithra','HR',100000);
  7  insert into empl (empid,empname,dept,salary)
  8  values (3,'sudhiksha','manager',200000);
  9  commit;
 10  end;
 11  /

Procedure created.

SQL> begin
  2  insert_empl_data;
  3  end;
  4  /

PL/SQL procedure successfully completed.

SQL> select * from empl;


```
### Output:
![image](https://github.com/RKavikeerthana/Ex-No-4-Creating-Procedures-using-PL-SQL/assets/120431120/d8d8fb47-a524-4ad2-8aa6-fb9c98b1a531)

### Result:
Hence the procedure using pl/sql is created successfully.
