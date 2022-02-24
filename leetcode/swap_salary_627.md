```sql
# update {table} set {column} = {value} where {condition}
UPDATE Salary SET sex =
CASE
    WHEN sex = "f" THEN "m"
    WHEN sex = "m" THEN "f"
END
```