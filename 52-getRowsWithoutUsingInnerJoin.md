---
layout: default
title: Get rows from multiple tables without using inner join
---

# Combine rows from different tables but do not require the join condition

`SELECT * FROM [table1] LEFT OUTER JOIN [table2] ON [table1].[column] = [table2].[column];`
*(The left table is the first table that appears in the statement.)*
