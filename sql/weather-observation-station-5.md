### Problem
https://www.hackerrank.com/challenges/weather-observation-station-5/problem
### Submit
```sql
(
  select CITY, length(CITY)
  from STATION
  where length(CITY) = (select min(length(CITY)) from STATION)
  order by CITY
  limit 1
)
union
(select CITY, length(CITY)
  from STATION
  where length(CITY) = (select max(length(CITY)) from STATION)
  order by CITY
  limit 1
)
```
