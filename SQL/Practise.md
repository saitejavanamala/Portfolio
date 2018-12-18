SQL practise

* Write a query to find the JobNumber, Status from Jobs table with ItemQty < 20


``` SQL
-- select the JobNumber, Status 
SELECT JobNumber, Status
FROM ptpdb1.Jobs
-- check ItemQty is less than 20
WHERE ItemQty < 20;
```

