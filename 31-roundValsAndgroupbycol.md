---
layout: default
title: Get 2 decimal average value and group values accordingly
---

# Get rounded average value and group by [category-column]

`SELECT [category-column],`<br />
`ROUND(AVG([column]), 2)`<br />
`FROM [table] GROUP BY [category-column];`
