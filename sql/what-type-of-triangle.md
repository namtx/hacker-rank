### Problem
https://www.hackerrank.com/challenges/what-type-of-triangle
### Submit
```sql
select
  case
    when (A + B <= C) or (A + C <= B) or (B + C <= A) then "Not A Triangle"
    when (A <> B) and (B <> C) and (C <> A) then "Scalene"
    when (A = B) and (B = C) then "Equilateral"
    when (A = B) or (B = C) or (C = A) then "Isosceles"
  end as 'Type'
from TRIANGLES
```
