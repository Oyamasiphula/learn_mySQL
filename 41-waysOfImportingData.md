---
layout: default
title: Ways of importing/restoring data
---

# Restore your database backup :relieved: <br />


Type the following command to import sql data file:

`mysql -u username -p -h localhost DATA-BASE-NAME < data.sql`


In this example, import 'data.sql' file into 'website' database using Sathish as username:

`mysql -u sat -p -h localhost blog < data.sql`


If you have a dedicated database server, replace localhost hostname with with actual server name or IP address as
follows:

`mysql -u username -p -h 202.54.1.10 databasename < data.sql`


OR use hostname such as mysql.cyberciti.biz

`mysql -u username -p -h mysql.cyberciti.biz database-name < data.sql`


If you do not know the database name or database name is included in sql dump you can try out something as follows:

`mysql -u username -p -h 202.54.1.10 < data.sql`
