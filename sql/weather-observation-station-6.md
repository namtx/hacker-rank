### Problem
https://www.hackerrank.com/challenges/weather-observation-station-6
### Submit
```sql
select CITY
from STATION
where (
      upper(left(CITY, 1)) = 'A'
  OR  upper(left(CITY, 1)) = 'E'
  OR  upper(left(CITY, 1)) = 'I'
  OR  upper(left(CITY, 1)) = 'O'
  OR  upper(left(CITY, 1)) = 'U'
)
```
