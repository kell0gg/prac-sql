```sql
# https://leetcode.com/problems/employees-earning-more-than-their-managers/
# 테이블이 하나니까 InnerJoin

SELECT a.name FROM Employee as e INNER JOIN Employee b ON a.managerId = b.id WHERE a.salary > b.salary
```