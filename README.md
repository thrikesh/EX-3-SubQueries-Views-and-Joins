# EX-3-SubQueries-Views-and-Joins
# Create employee Table

CREATE TABLE EMP (EMPNO NUMBER(4) PRIMARY KEY,ENAME VARCHAR2(10),JOB VARCHAR2(9),MGR NUMBER(4),HIREDATE DATE,SAL NUMBER(7,2),COMM NUMBER(7,2),DEPTNO NUMBER(2));
Insert the values

INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO) VALUES (7369, 'SMITH', 'CLERK', 7902, '17-DEC-80', 800, NULL, 20);

INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO) VALUES (7499, 'ALLEN', 'SALESMAN', 7698, '20-FEB-81', 1600, 300, 30);

INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO) VALUES (7521, 'WARD', 'SALESMAN', 7698, '22-FEB-81', 1250, 500, 30);

INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO) VALUES (7566, 'JONES', 'MANAGER', 7839, '02-APR-81', 2975, NULL, 20);

INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO) VALUES (7654, 'MARTIN', 'SALESMAN', 7698, '28-SEP-81', 1250, 1400, 30);

INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO) VALUES (7698, 'BLAKE', 'MANAGER', 7839, '01-MAY-81', 2850, NULL, 30);

INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO) VALUES (7782, 'CLARK', 'MANAGER', 7839, '09-JUN-81', 2450, NULL, 10);

INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO) VALUES (7788, 'SCOTT', 'ANALYST', 7566, '19-APR-87', 3000, NULL, 20);

INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO) VALUES (7839, 'KING', 'PRESIDENT', NULL, '17-NOV-81', 5000, NULL, 10);

INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO) VALUES (7844, 'TURNER', 'SALESMAN', 7698, '08-SEP-81', 1500, 0, 30);

INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO) VALUES (7876, 'ADAMS', 'CLERK', 7788, '23-MAY-87', 1100, NULL, 20);

INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO) VALUES (7900, 'JAMES', 'CLERK', 7698, '03-DEC-81', 950, NULL, 30);

INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO) VALUES (7902, 'FORD', 'ANALYST', 7566, TO_DATE('03-DEC-81', 'DD-MON-RR'), 3000, 20, 20);

INSERT INTO EMP (EMPNO, ENAME, JOB, MGR, HIREDATE, SAL, COMM, DEPTNO) VALUES (7934, 'MILLER', 'CLERK', 7782, TO_DATE('23-JAN-82', 'DD-MON-RR'), 1300, 10, 10);
Create department table

CREATE TABLE DEPT (DEPTNO NUMBER(2) PRIMARY KEY,DNAME VARCHAR2(14),LOC VARCHAR2(13));
Insert the values in the department table

INSERT INTO DEPT (DEPTNO, DNAME, LOC) VALUES (10, 'ACCOUNTING', 'NEW YORK');

INSERT INTO DEPT (DEPTNO, DNAME, LOC) VALUES (20, 'RESEARCH', 'DALLAS');

INSERT INTO DEPT (DEPTNO, DNAME, LOC) VALUES (30, 'SALES', 'CHICAGO');

INSERT INTO DEPT (DEPTNO, DNAME, LOC) VALUES (40, 'OPERATIONS', 'BOSTON');
Q1) List the name of the employees whose salary is greater than that of employee with empno 7566.
# QUERY:
<br>
<img width="625" alt="271338255-4da768df-84f3-4a8c-85aa-1e184b5d672c" src="https://github.com/thrikesh/EX-3-SubQueries-Views-and-Joins/assets/119576222/3fe4e079-e157-4da2-a4e7-c1e74cd3b51d">

# OUTPUT:
<br>
<img width="142" alt="271338426-b8622f9f-3faf-4218-a971-832c0028ca68" src="https://github.com/thrikesh/EX-3-SubQueries-Views-and-Joins/assets/119576222/75ca3058-3f4f-4989-a8f1-ff58d8034f3b">

Q2) List the ename,job,sal of the employee who get minimum salary in the company.
# QUERY:
<br>
<img width="578" alt="271338751-e9647973-af79-4a1e-a179-7b284c225d0b" src="https://github.com/thrikesh/EX-3-SubQueries-Views-and-Joins/assets/119576222/01126c2e-9cd5-45e9-89fe-8bb5dd30bca0">


# OUTPUT:
<br>
<img width="317" alt="271338909-6235cc68-e4dd-4965-a696-d94b63b9adfa" src="https://github.com/thrikesh/EX-3-SubQueries-Views-and-Joins/assets/119576222/16d72628-c23c-451d-a36a-4fb71616869a">


Q3) List ename, job of the employees who work in deptno 10 and his/her job is any one of the job in the department ‘SALES’.
# QUERY:
<br>
<img width="634" alt="271339101-af237eb7-efb2-4a04-8e0b-d6b8997ce0da" src="https://github.com/thrikesh/EX-3-SubQueries-Views-and-Joins/assets/119576222/b5264329-421c-4321-b81a-c6429fe6b303">


# OUTPUT:
<br>
<img width="163" alt="271339283-70e7db53-9cee-417f-b12c-32e3d1438b92" src="https://github.com/thrikesh/EX-3-SubQueries-Views-and-Joins/assets/119576222/52cb72ee-9ef1-4038-b84f-01a583b1335f">

Q4) Create a view empv5 (for the table emp) that contains empno, ename, job of the employees who work in dept 10.
# QUERY:
<br>
<img width="628" alt="271339490-4d60f20e-18a0-432a-abfd-0da8334b07e9" src="https://github.com/thrikesh/EX-3-SubQueries-Views-and-Joins/assets/119576222/a505a1d4-6470-4c47-9531-d851267f2a7b">

# OUTPUT:
<br>
<img width="141" alt="271339617-2cc9bbed-e2a9-4566-bf70-fb71e626da08" src="https://github.com/thrikesh/EX-3-SubQueries-Views-and-Joins/assets/119576222/8580c03d-34a0-4c3d-9b13-7be82fbaa4b6">

Q5) Create a view with column aliases empv30 that contains empno, ename, sal of the employees who work in dept 30. Also display the contents of the view.
# QUERY:
<br>
<img width="631" alt="271339811-0210d44a-5c6d-4ff6-a2b3-9f0ef1be5cf3" src="https://github.com/thrikesh/EX-3-SubQueries-Views-and-Joins/assets/119576222/90b773f9-6994-4bbc-95c2-501fbf0a57ab">

# OUTPUT:
<br>
<img width="377" alt="271340001-d792f018-fd12-4b38-a976-23eec0c0d416" src="https://github.com/thrikesh/EX-3-SubQueries-Views-and-Joins/assets/119576222/6d9e6383-9e5d-4117-bc01-9c4dab9cbd81">



Q6) Update the view empv5 by increasing 10% salary of the employees who work as ‘CLERK’. Also confirm the modifications in emp table
# QUERY:
<br>
<img width="547" alt="271340210-da284c6e-6627-4237-a92a-69e5d8fdc09f" src="https://github.com/thrikesh/EX-3-SubQueries-Views-and-Joins/assets/119576222/640f7795-b219-4ba7-af75-107a11884ebb">


# OUTPUT:
<br>
<img width="376" alt="271340362-f5cd1cff-d99e-441e-9c6f-a4b468552a41" src="https://github.com/thrikesh/EX-3-SubQueries-Views-and-Joins/assets/119576222/6ab67d08-24da-47c5-b32c-32ceeec4df34">

# Create a Customer1 Table

CREATE TABLE Customer1 (customer_id INT,cust_name VARCHAR(20),city VARCHAR(20),grade INT,salesman_id INT);
Inserting Values to the Table

INSERT INTO Customer1 (customer_id, cust_name, city, grade, salesman_id) VALUES(3002, 'Nick Rimando', 'New York', 100, 5001); INSERT INTO Customer1 (customer_id, cust_name, city, grade, salesman_id) VALUES(3007, 'Brad Davis', 'New York', 200, 5001); INSERT INTO Customer1 (customer_id, cust_name, city, grade, salesman_id) VALUES(3005, 'Graham Zusi', 'California', 200, 5002); INSERT INTO Customer1 (customer_id, cust_name, city, grade, salesman_id) VALUES(3008, 'Julian Green', 'London', 300, 5002); INSERT INTO Customer1 (customer_id, cust_name, city, grade, salesman_id) VALUES(3004, 'Fabian Johnson', 'Paris', 300, 5006); INSERT INTO Customer1 (customer_id, cust_name, city, grade, salesman_id) VALUES(3009, 'Geoff Cameron', 'Berlin', 100, 5003); INSERT INTO Customer1 (customer_id, cust_name, city, grade, salesman_id) VALUES(3003, 'Jozy Altidor', 'Moscow', 200, 5007); INSERT INTO Customer1 (customer_id, cust_name, city, grade, salesman_id) VALUES(3001, 'Brad Guzan', 'London', NULL, 5005);
Create a Salesperson1 table

CREATE TABLE Salesman1 (salesman_id INT,name VARCHAR(20),city VARCHAR(20),commission DECIMAL(4,2));
Inserting Values to the Table

INSERT INTO Salesman1 (salesman_id, name, city, commission) VALUES(5001, 'James Hoog', 'New York', 0.15); INSERT INTO Salesman1 (salesman_id, name, city, commission) VALUES(5002, 'Nail Knite', 'Paris', 0.13); INSERT INTO Salesman1 (salesman_id, name, city, commission) VALUES(5005, 'Pit Alex', 'London', 0.11); INSERT INTO Salesman1 (salesman_id, name, city, commission) VALUES(5006, 'Mc Lyon', 'Paris', 0.14); INSERT INTO Salesman1 (salesman_id, name, city, commission) VALUES(5007, 'Paul Adam', 'Rome', 0.13); INSERT INTO Salesman1 (salesman_id, name, city, commission) VALUES(5003, 'Lauson Hen', 'San Jose', 0.12);
Q7) Write a SQL query to find the salesperson and customer who reside in the same city. Return Salesman, cust_name and city.
# QUERY:
<br>
<img width="637" alt="271340967-c452ad5c-1a03-4b96-acc6-9262689b0174" src="https://github.com/thrikesh/EX-3-SubQueries-Views-and-Joins/assets/119576222/c7c7b8d9-7579-4742-8e74-7f49f2cc34ef">


# OUTPUT:
<br>
<img width="570" alt="271341099-307dd60f-ef3c-400a-b8b1-ee64b7ed2c29" src="https://github.com/thrikesh/EX-3-SubQueries-Views-and-Joins/assets/119576222/81b3b74b-94ad-4d9d-b077-49f7613e133f">

Q8) Write a SQL query to find salespeople who received commissions of more than 13 percent from the company. Return Customer Name, customer city, Salesman, commission.
# QUERY:
<br>
<img width="638" alt="271341282-2c628085-5574-43fc-8864-3d4752eb3663" src="https://github.com/thrikesh/EX-3-SubQueries-Views-and-Joins/assets/119576222/4cfeb22e-6e60-4568-bbdb-2702e0b70fff">


# OUTPUT:
<br>
<img width="629" alt="271341444-87e9b5f0-3ea2-439f-af92-c2e5833c9e20" src="https://github.com/thrikesh/EX-3-SubQueries-Views-and-Joins/assets/119576222/52b210d0-b106-499d-8612-46c52df0695a">


Q9) Perform Natural join on both tables
# QUERY:
<br>
<img width="637" alt="271341692-1c7bdf18-bebd-47be-93a8-83e026886801" src="https://github.com/thrikesh/EX-3-SubQueries-Views-and-Joins/assets/119576222/63b455ed-44c3-4d01-b573-6e60b3ab9353">

# OUTPUT:
<br>
<img width="637" alt="271341834-5a33d1e3-333d-4d16-8d72-cf9243281678" src="https://github.com/thrikesh/EX-3-SubQueries-Views-and-Joins/assets/119576222/df0db24e-abf9-417d-9a36-dffa29ff931c">

Q10) Perform Left and right join on both tables
# OUTPUT:
# Left Join
<br>
<img width="631" alt="271342626-c6736840-cc86-42ea-9b1c-3b0004d8bc02" src="https://github.com/thrikesh/EX-3-SubQueries-Views-and-Joins/assets/119576222/f14b8e64-88e0-4783-85e0-0ff6369a2e99">

# Right Join
<br>
<img width="599" alt="271342865-290ef10d-70af-44a8-9654-8c96ed4e0cc5" src="https://github.com/thrikesh/EX-3-SubQueries-Views-and-Joins/assets/119576222/363c85a2-7a4e-4663-a946-61c436c2760f">
