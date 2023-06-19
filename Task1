#Table with Student Details.
create table students(ID int,NAME varchar(20));

#Inserting values in the table.
insert into students values(1,'Rithish');
insert into students values(2,'Jhon');

#Adding columns in the table.
alter table students add GENDER char;
alter table students add MOBILE_NO int;
alter table students add Dept varchar(10);
alter table students add CGPA double;

#Updating values to the newly created column.
update students set gender="M",MOBILE_NO=8870505405,Dept="CSE",CGPA=8.7 where id=1;
update students set gender="M",MOBILE_NO=9994293893,Dept="AIDS",CGPA=7.9 where id=2;
insert into students (Id,NAME,GENDER,MOBILE_NO,Dept,CGPA)
values (3,"Roopak","M",8594637564,"ECE",8.4),
       (4,"Saran","M",9993372746,"EEE",7.4),
       (5,"Natrajan","M",9475463546,"ECE",9.1),
       (6,"Jeysu","F",9473546574,"CSE",8.2),
       (7,"swathi","F",8455736476,"EEE",9.3),
       (8,"yasotha","F",6753844758,"CSE",7.1),
       (9,"Mani","M",8973546578,"ECE",7.9),
       (10,"Aakash","M",9004537465,"EEE",8.3);
select * from students where id=1;
alter table students drop gender;
select * from students where id between 6 and 7;
select * from students order by NAME desc;

#Avg
select avg(CGPA) as AVG_CGPA from students;
#MAX
select name,max(CGPA) from students;
#MIN
select name,min(CGPA) from students;
#COUNT
select count(Id) from students;

#Table with Faculty Information.
create table Faculty(F_id int,F_Name varchar(20),Dept varchar(10));
insert into Faculty(F_id,F_Name,Dept) 
values(1,"Henry","CSE"),
      (2,"Mark","ECE"),
      (3,"Carol","EEE");
      
#Joining Student Table and Faculty Table.
select Faculty.F_Name,Faculty.Dept,Students.NAME,Students.CGPA from Faculty Join
Students where Faculty.Dept=Students.Dept;
