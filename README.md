# sql-Practice-1-bY-Vimal-Kumar

create database Project
use Project
 create table Employee(id int primary key identity(101,1),F_Name varchar(80),L_Name varchar(50),
 salary int,Department_Name varchar(60),Gender varchar(20),Department_No int )

 INSERT INTO Employee values
 ('Rejesh','Singh',30000,'IT','Male'),
('Vimla','kumari',15000,'HR','Female'),
 ('Mohan','Singh',25000,'HR','Male'),
 ('Sohan','Gopal',15000,'TL','Male'),
 ('Yuvika','Singh',10000,'IT','Female'),
 ('Vikas','Kumar',9000,'IT','Male'),
 ('Rubi','Rani',8000,'IT','Female')


 UPDATE Employee SET Department_No=8 WHERE id=101
  UPDATE Employee SET Department_No=9 WHERE id=102
   UPDATE Employee SET Department_No=10 WHERE id=103
  UPDATE Employee SET Department_No=12 WHERE id=104
   UPDATE Employee SET Department_No=13 WHERE id=105
    UPDATE Employee SET Department_No=14 WHERE id=106
	 UPDATE Employee SET Department_No=15 WHERE id=107

 select*from Employee

 select*from Employee where salary<10000

 select*from Employee where salary>=9000 AND salary<15000 


 select*from Employee where salary NOT BETWEEN 9000 AND 15000


 select*from Employee where F_Name LIKE 'r%'

select*from Employee where F_Name LIKE '%u'

select*from Employee where F_Name LIKE '%a%'

select*from Employee where F_Name LIKE '____'

select*from Employee where F_Name LIKE '%r%' AND salary>9000 

select*from Employee where salary>
(select salary from Employee where F_Name='raju')

select*from Employee where id like '1%1'


 UPDATE Employee SET Department_No=10 WHERE id IN(101,103,107)

UPDATE Employee SET Department_No=8 WHERE id=101



UPDATE Employee SET Department_No=20 WHERE  DEPT_NO=null

UPDATE Employee SET SALARY=20000 WHERE Department_No>10 and F_Name LIKE 'R%'

UPDATE Employee SET Department_No=30 WHERE F_Name LIKE 'm%'

UPDATE Employee SET salary=8500 WHERE Department_No not between 10 and 30

select*from Employee

 UPDATE Employee SET SALARY=15000 WHERE Department_No>10 and F_Name LIKE 'R%'

  UPDATE Employee SET SALARY=5500 WHERE Department_No<20 and id>105


UPDATE Employee SET SALARY=25000 WHERE SALARY<10000 and F_Name LIKE '%R%' and  DEPT_NO<20 


UPDATE Employee SET SALARY=10000 WHERE SALARY>=8500 and  SALARY<=15000
