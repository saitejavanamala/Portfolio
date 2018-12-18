SQL practise

* Write a query to find the JobNumber, Status from Jobs table with ItemQty < 20


``` SQL
-- select the JobNumber, Status 
SELECT JobNumber, Status
FROM ptpdb1.Jobs
-- check ItemQty is less than 20
WHERE ItemQty < 20;
```

* Write a query to find the JobNumber, ContractDate from Jobs table where Status is 'WG', 'WS', or 'WP' and Size is 1 or 4

``` SQL
-- select the JobNumber, ContractDate
SELECT JobNumber, ContractDate
FROM ptpdb1.Jobs
-- check Status is 'WG', 'WS', or 'WP'
-- check that  Size is 1 or 4
WHERE Status IN ('WG', 'WS', or 'WP') AND Size IN (1, 4);

```
