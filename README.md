

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


```sql
alter table world 
alter column 日期 type date
using 日期::DATE;

select 洲名,國家,日期,總確診數,總死亡數,新增死亡數
from world;


select max(總確診數) as 總確診數
from world
where 國家='台灣'and 日期 between'2020-01-01'and'2020-12-31';
```