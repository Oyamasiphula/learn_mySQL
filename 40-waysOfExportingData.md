---
layout: default
title: Ways of exporting/download data
---

#Create a backup of your data or copy your data :relaxed: <br />

If it's an entire DB, then:

`mysqldump -u [uname] -p[pass] db_name > db_backup.sql`


If it's all DBs, then:

`mysqldump -u [uname] -p[pass] --all-databases > all_db_backup.sql`


If it's specific tables within a DB, then:

`mysqldump -u [uname] -p[pass] db_name table1 table2 > table_backup.sql`


You can even go as far as auto-compressing the output using gzip (if your DB is very big):

`mysqldump -u [uname] -p[pass] db_name | gzip > db_backup.sql.gz`


If you want to do this remotely and you have the access to the server in question, then the following would work (presuming the MySQL server is on port 3306):

`mysqldump -P 3306 -h [ip_address] -u [uname] -p[pass]`
