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
  cat.ID,
  cat.NAME AS SUPERCATEGORY_NAME,
  scat.NAME AS CATEGORY_NAME
FROM
  personalfinance.DIMPRDCATEGORY cat
  LEFT JOIN personalfinance.DIMPRDCATEGORY scat ON cat.ID = scat.SUPERCATEGORYID;
```	