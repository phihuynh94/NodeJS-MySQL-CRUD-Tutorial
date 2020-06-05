# NodeJS-MySQL-CRUD-Tutorial

Tech: Nodejs - mySQL

Tutorial: https://www.youtube.com/watch?v=4fWWn2Pe2Mk&t=142s

MySql query:

  Create employee table:
  
    use employeeDB;

    CREATE table employee (
      empID int(11) not null auto_increment,
        name varchar(45) default null,
        empCode varchar(45) default null,
        salary int(11) default null,
        primary key(empID)
    ) engine=InnoDB auto_increment=0 default charset=utf8mb4 collate=utf8mb4_0900_ai_ci;
    
  Fill in data:
    
    use employeedb;

    lock tables employee write;
    insert into employee values (1, 'Gavin Cortez', 'EMP90', 265400), (2,'Quinn Flynn','EMP94',364600),(3,'Doris  Wilder','EMP06',316400),(4,'Hermione Butler','EMP965',417500);
    unlock tables;
    
