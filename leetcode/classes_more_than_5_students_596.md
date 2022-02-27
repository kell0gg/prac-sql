```sql
SELECT c.class FROM Courses as c GROUP BY c.class HAVING COUNT(DISTINCT student) >= 5;
```