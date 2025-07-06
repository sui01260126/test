

```sql
create table if not exists student(
student_id SERIAL primary key,
name varchar(20) not null,
major varchar(20) unique
);

drop table if exists student;
```
INSERT INTO STUDENT(NAME,MAJOR)
VALUES('小柱','生物'),('信忠','英語');

INSERT INTO STUDENT(NAME,MAJOR)
VALUES('小王','國文');

select STUDENT_ID,NAME,MAJOR
from STUDENT
where NAME='小柱'
order by STUDENT_ID desc;
```