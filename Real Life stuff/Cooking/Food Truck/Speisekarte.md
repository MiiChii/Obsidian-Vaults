```dataview
TABLE without id file.link AS Dish, kitchen AS Kitchen, type AS Category
FROM #recipe AND #foodtruck
WHERE file.name != "Recipe"
SORT kitchen asc
```