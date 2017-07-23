### Problem
https://www.hackerrank.com/challenges/occupations/problem
### Submit
```sql
set @p=0, @a=0, @d=0, @s=0;
select min(Doctor), min(Professor), min(Singer), min(Actor)
from
(
  select
  case OCCUPATION
    when "Professor" then @p := @p + 1
    when "Actor" then @a := @a + 1
    when "Doctor" then @d:= @d + 1
    when "Singer" then @s:= @s + 1
  end as ROW_NUMBER,
  case when OCCUPATION="Professor" then NAME end as Professor,
  case when OCCUPATION="Doctor" then NAME end as Doctor,
  case when OCCUPATION="Actor" then NAME end as Actor,
  case when OCCUPATION="Singer" then NAME end as Singer
  from OCCUPATIONS
  order by NAME
) Temp
group by ROW_NUMBER
```
