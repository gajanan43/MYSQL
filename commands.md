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
15) 
