### Problem
https://www.hackerrank.com/challenges/the-pads/problem
### Submit
```sql
select concat(NAME, concat("(", concat(left(OCCUPATION, 1), ")"))) as NAME
from OCCUPATIONS
order by NAME;

select concat("There are a total of ", concat(count(OCCUPATION), concat(" ", concat(lower(OCCUPATION), "s.")))) as NAME
from OCCUPATIONS
group by OCCUPATION
order by count(OCCUPATION), OCCUPATION
```
