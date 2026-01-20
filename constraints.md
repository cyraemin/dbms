## Constraints
1. Primary key
(not null + unique)
used to identify each row
uniquely identifies each row

2. Not Null
column must have a value
eg-name text not null
3. Unique
no duplicate values allowed
eg-email text unique
4. Default
provides default value if none
eg-created_at timestamp default now()

5. Check
validates values
eg-age int check (age >= 18)
6. Foreign key
links one table to another
eg-user_id int references users(id)



create table random (
id serial primary key,
name varchar(100) not null,
email text unique,
created_at date default now(),
age int check (age >= 18)
);
insert into random (name, age)
values ('Aseesh', 23);