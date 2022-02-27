```sql
# 가장 큰 값보다 작은 애들 중에 제일 높은 애
SELECT MAX(Salary) as SecondHighestSalary FROM Employee WHERE Salary < (Select MAX(Salary) FROM Employee);
```