---
title: mysql create user and grant permissions
date: 2021-07-26 16:11:45
tags: [mysql]
---

```sql
CREATE USER 'powerdata'@'%' IDENTIFIED BY 'admin';
GRANT ALL PRIVILEGES ON *.* TO 'powerdata'@'%' WITH GRANT OPTION;
FLUSH PRIVILEGES;

ALTER USER 'powerdata'@'%' IDENTIFIED BY 'admin'

```

some time you encounter error like:

```
[Err] 1055 - Expression #1 of ORDER BY clause is not in GROUP BY clause and contains nonaggregated column 'information_schema.PROFILING.SEQ' which is not functionally dependent on columns in GROUP BY clause; this is incompatible with sql_mode=only_full_group_by
```

use follow sql:

```sql

select version(), @@sql_mode;SET sql_mode=(SELECT REPLACE(@@sql_mode,'ONLY_FULL_GROUP_BY',''));

```
