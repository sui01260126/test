

```sql
create table if not exists student(
student_id SERIAL primary key,
name varchar(20) not null,
major varchar(20) unique
);

drop table if exists students;
```
INSERT INTO STUDENT(NAME,MALOR)
VALUES('小柱','生物')('信忠','英語')