# Commands:

1) create database DB_NAME;
2) use DB_NAME;
3) show databases;
4) drop database DB_NAME
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
23)  
