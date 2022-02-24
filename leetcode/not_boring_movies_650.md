```sql
# id가 홀수이고, description이 boring이 아니면 됨
SELECT c.id, c.movie, c.description, c.rating FROM CINEMA as c WHERE (c.id % 2 = 1) AND c.description != "boring" ORDER BY c.rating DESC;
```