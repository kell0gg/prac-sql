```sql
# https://leetcode.com/problems/duplicate-emails/
# 중복제거 -> 2번 이상 나온 값들을 확인해야 함 -> GROUP BY, HAVING 사용

SELECT email as `Email` FROM Person GROUP BY email HAVING count(*) > 1
```

```sql
SELECT * FROM Person GROUP BY email

# {"headers": ["id", "email"], "values": [[1, "a@b.com"], [2, "c@d.com"]]}
```