### Problem
https://www.hackerrank.com/challenges/binary-search-tree-1/problem
### Submit
```sql
select
  N,
  if(P IS null, 'Root', if((select count(*) from BST B where B.P = BST.N) > 0, 'Inner', 'Leaf'))
from BST
order by N
```
