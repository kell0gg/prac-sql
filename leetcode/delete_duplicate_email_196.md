```sql
# NOT IN + SUB QUERY
DELETE FROM PERSON WHERE id NOT IN
(SELECT A.id FROM (SELECT MIN(id) as Id from Person GROUP BY Email) as A);
```