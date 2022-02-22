```sql
# https://leetcode.com/problems/combine-two-tables/
# Persion ID를 가지고 JOIN

SELECT p.firstName, p.lastName,  a.city, a.state FROM Person as p LEFT JOIN Address as a ON p.personId = a.personId;
```

