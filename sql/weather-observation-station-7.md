### Problem
https://www.hackerrank.com/challenges/weather-observation-station-7
### Submit
```sql
select distinct CITY
from STATION
where (
      upper(right(CITY, 1)) = 'A'
  OR  upper(right(CITY, 1)) = 'E'
  OR  upper(right(CITY, 1)) = 'I'
  OR  upper(right(CITY, 1)) = 'O'
  OR  upper(right(CITY, 1)) = 'U'
)
```
