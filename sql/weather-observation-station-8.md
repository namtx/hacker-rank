### Problem
https://www.hackerrank.com/challenges/weather-observation-station-8
### Submit
```sql
select distinct CITY
from STATION
where (
  (    
        upper(left(CITY, 1)) = 'A'
    OR  upper(left(CITY, 1)) = 'E'
    OR  upper(left(CITY, 1)) = 'I'
    OR  upper(left(CITY, 1)) = 'O'
    OR  upper(left(CITY, 1)) = 'U'
  )
  AND
  (    
        upper(right(CITY, 1)) = 'A'
    OR  upper(right(CITY, 1)) = 'E'
    OR  upper(right(CITY, 1)) = 'I'
    OR  upper(right(CITY, 1)) = 'O'
    OR  upper(right(CITY, 1)) = 'U'
  )
) 
```
