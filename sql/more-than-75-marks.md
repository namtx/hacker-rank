### Problem
https://www.hackerrank.com/challenges/more-than-75-marks
### Submit
```sql
select STUDENTS.NAME
from STUDENTS
where
(
  STUDENTS.MARKS > 75
)
order by right(STUDENTS.NAME, 3), STUDENTS.ID
```
