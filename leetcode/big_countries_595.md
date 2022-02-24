```sql
# 단일 테이블, 별도 조인 없이 WHERE로 처리

SELECT w.name, w.population, w.area FROM World as w WHERE w.area >= 3000000 OR w.population >= 25000000;
```