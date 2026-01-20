## Data Types in SQL
1. Numeric DT
2. Character / String DT
3. Boolean Type
4. Date and Time Types


1. Numeric
a. Smallint
-2 bytes integer
-Range: -32768 to 32767

b. Integer / Int
-4 bytes integer
c. Bigint
-8 bytes integer
-Used when very large numbers are required
d. Decimal (p, s)
-Exact precision
e. Numeric (p, s)
-Exact precision
-p = total number of digits
-s = number of digits after decimal point
f. Real
-4-byte floating point
-Used for rating, real values
g. Double Precision
-8-byte floating point
-More accurate than real
h. Serial
-Auto-increment integer
-Used as id (serial)


Example:
create table numbers (
id serial,
age int,
price numeric(4,2),
rating real
);
insert into numbers (age, price, rating)
values
(20, 20.25, 7.777),
(19, 69.75, 7.778);

2. Character / String
a. char(n)
--Fixed length
Example: code char(5) -> 'hi   '
b. varchar(n)
-Variable length string
-Limit is required
-Example: email varchar(100)
c. text
-Unlimited length
-Example: bio text


Example:
create table string (
code char(5),
email varchar(100),
bio text
);
insert into string
values ('12345', 'tamsilsameera@gmail.com', 'this is an exam');

3. Boolean
Boolean
-true,false,null
Example:
is_active boolean

4. Date and Time
a. Date
-Stores only date
-Format: 2025-01-05
b. Time
-Stores only time
-Format: 14:30:00
c. Timestamp
-Stores date and time
d.Timestampz-
Stores date, time, and timezone
e. Interval
-Stores time difference