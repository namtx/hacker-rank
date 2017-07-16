### Problem
https://www.hackerrank.com/challenges/weather-observation-station-9
### Submit
```sql
select distinct CITY
from STATION
where (
       upper(left(CITY, 1)) <> 'A'
  AND  upper(left(CITY, 1)) <> 'E'
  AND  upper(left(CITY, 1)) <> 'I'
  AND  upper(left(CITY, 1)) <> 'O'
  AND  upper(left(CITY, 1)) <> 'U'
)
```
