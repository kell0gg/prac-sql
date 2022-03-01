```sql
SELECT id, 
	SUM(CASE WHEN month = 'jan' then revenue ELSE null END) as Jan_Revenue,
	SUM(CASE WHEN month = 'feb' then revenue ELSE null END) as Feb_Revenue,
	SUM(CASE WHEN month = 'mar' then revenue ELSE null END) as Mar_Revenue,
	SUM(CASE WHEN month = 'apr' then revenue ELSE null END) as Apr_Revenue,
	SUM(CASE WHEN month = 'may' then revenue ELSE null END) as May_Revenue,
	SUM(CASE WHEN month = 'jun' then revenue ELSE null END) as Jun_Revenue,
	SUM(CASE WHEN month = 'jul' then revenue ELSE null END) as Jul_Revenue,
	SUM(CASE WHEN month = 'aug' then revenue ELSE null END) as Aug_Revenue,
	SUM(CASE WHEN month = 'sep' then revenue ELSE null END) as Sep_Revenue,
	SUM(CASE WHEN month = 'oct' then revenue ELSE null END) as Oct_Revenue,
	SUM(CASE WHEN month = 'nov' then revenue ELSE null END) as Nov_Revenue,
	SUM(CASE WHEN month = 'dec' then revenue ELSE null END) as Dec_Revenue
FROM Department
GROUP BY id
ORDER BY id
```