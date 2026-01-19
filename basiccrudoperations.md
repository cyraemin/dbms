## Basic CRUD operations
1. To create database
Create Database new_db;

2. To create table
create table students (
    student_id INT,
    name char (50),
    age INT,
    grade char (1)
);

3. Now to insert values
Insert into students (name, age, grade)
values ('Sam', 20, 'A');
       ('apple', 19, 'A');

4. To read table
select * from students;

5. for specific column
select name from students;
select name from students where age = 23;

6. To update - update, set, where
update table students
set age = 25
where name = 'apple';

7. To delete
delete from students
where name = 'Sam';