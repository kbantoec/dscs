# MySQL

## Create a table with recursion

```sql
CREATE TABLE `personalfinance`.`DIMPRDCATEGORY` (
  `ID` INT NOT NULL AUTO_INCREMENT,
  `NAME` VARCHAR(30) NOT NULL,
  `SUPERCATEGORYID` INT NULL,
  PRIMARY KEY (`ID`));
```

```sql
SELECT
  cat1.ID,
  cat1.NAME AS CATEGORY_NAME_1,
  cat2.NAME AS CATEGORY_NAME_2,
  cat3.NAME AS CATEGORY_NAME_3
FROM
  personalfinance.DIMPRDCATEGORY cat1
  LEFT JOIN personalfinance.DIMPRDCATEGORY cat2 ON cat1.ID = cat2.SUPERCATEGORYID
  LEFT JOIN personalfinance.DIMPRDCATEGORY cat3 ON cat2.ID = cat3.SUPERCATEGORYID
WHERE 1=1
AND cat1.SUPERCATEGORYID IS NULL
ORDER BY
 1, 2, 3, 4;
```

How to change (update) a value in a table:
```sql
UPDATE personalfinance.DIMPRDCATEGORY
SET `SUPERCATEGORYID` = 1
WHERE `NAME` = 'health insurance';
```