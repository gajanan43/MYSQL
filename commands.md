# Commands:

1) create database DB_NAME;
2) USE DB_NAME;
3) SHOW databases;
4) DROP database DB_NAME
5) create table users(id INT AUTO_INCREMENT PRIMARY KEY, name VARCHAR(50) NOT NULL,email VARCHAR(50) UNIQUE NOT NULL);
6) show tables;
7) select*from TB_NAME;
8) select COL1,COL2 from TB_NAME;
9) rename table OLD_TB_NAME to NEW_TB_NAME;
10) alter table TB_NAME ADD NEW_COL_NAME DATA_TYPE;
11) alter table TB_NAME drop column COL_NAME;
12) alter table TB_NAME MODIFY column COL_NAME CHANGE_DATA_TYPE(varchar(150));
13) alter table TB_NAME MODIFY column COL3 DATA_TYPE after COL1;
14) insert into TB_NAME values(1,"Gajanan","demo@gmail.com");
15) select*from TB_NAME where CONDITION(id<3);
16) select*from TB_NAME where id BETWEEN 1 AND 4;
17) select*from TB_NAME where id IN(1,4);
18) select*from TB_NAME where gender="male" AND salary>70000;
19) select*from TB_NAME where gender="male" OR salary>70000;
20) select*from TB_NAME where gender="male" OR salary>70000 ORDER BY COL_NAME ASC;
21) select*from TB_NAME where gender="male" OR salary>70000 ORDER BY COL_NAME DESC;
22) select*from TB_NAME where gender="male" OR salary>70000 ORDER BY COL_NAME DESC LIMIT 5;
23) UPDATE TB_NAME set salary=45000 where id=1;
24) DELETE from TB_NAME where id=25;
25) DROP table TB_NAME;
26) select COUNT(*) from TB_NAME;
27) select MIN(salary) AS Min_Salary, MAX(salary) AS Max_Salary from TB_NAME;
28) select SUM(salary) AS Toatl from TB_NAME;
29) select AVG(salary) AS Average from TB_NAME;
30) select gender,SUM(salary) AS avg from TB_NAME GROUP BY gender;
31) select gender,name, LENGTH(name) AS name_len from TB_NAME;
32) select id,gender,LOWER(name) AS lower,CONCAT(LOWER(name),"5677") AS username from TB_NAME;
33) select student.name,student.gender,addresses.city,addresses.state from student INNER JOIN addresses ON student.id=addresses.user_id;
34) select student.name,student.gender,addresses.city,addresses.state from student LEFT JOIN addresses ON student.id=addresses.user_id;
35) select student.name,student.gender,addresses.city,addresses.state from student RIGHT JOIN addresses ON student.id=addresses.user_id;
36) select name from student UNION  select name from admin_users;  -> show single list of unique names;
37) select name from student UNION ALL  select name from admin_users;  -> show single list of duplicate names;
38) create VIEW rich_users AS select*from student where salary>70000;
39) DROP view rich_users;
40) show INDEXES from TB_NAME;
41) select*from student where salary > (select avg(salary) from student);  -> show users how have more salary than average salary
42) select gender,avg(salary) from student GROUP BY gender;
43) select gender,AVG(salary) AS 'average', COUNT(*) AS 'Count' from student GROUP BY gender;
44) select gender,AVG(salary) AS 'average', COUNT(*) AS 'Count' from student GROUP BY gender HAVING AVG(salary)>62000;
45) select gender,AVG(salary) AS 'average', COUNT(*) AS 'Count' from student WHERE id<15 GROUP BY gender HAVING AVG(salary)>62000;
    
