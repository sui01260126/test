123


```sql
create table if not exists student(
student_id SERIAL primary key,
name varchar(20) not null,
major varchar(20) unique
);

drop table if exists students;
```
