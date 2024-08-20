---
tags:
  - ingredients
icon: LiContainer
---

```dataview
TASK
FROM #ingredients
SORT DESC
GROUP BY alias
SORT choice(alias = "Spices", "1" , 
	choice(alias = "Oil", "2", 
	choice(alias = "Sauces", "3", 
	choice(alias = "Vinegar", "4", 
	choice(alias = "Canned Goods", "5", 
	choice(alias = "Veggies", "6", 
	choice(alias = "Grains", "7", 
	choice(alias = "Baking", "8", "9"
	)))))))) ASC
```