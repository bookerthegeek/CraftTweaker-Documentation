# Alloy Smelter
## Calling The Package
You can call the AlloySmelter package using `mods.techreborn.alloySmelter`

Addition
------
```java
mods.techreborn.alloySmelter.addRecipe(ItemStack input1, ItemStack input2, ItemStack output1, int tickTime, int euPerTick);
mods.techreborn.alloySmelter.addRecipe(<minecraft:dirt>, <minecraft:sand>, <minecraft:diamond>, 40, 500);
```

```java
mods.techreborn.alloySmelter.removeRecipe(IItemStack output);
```

```java
mods.techreborn.alloySmelter.addRecipe(IItemStack output, IIngredient input1, IIngredient input2, int ticktime, int euTick);
```


Removal
------
```java
mods.techreborn.alloySmelter.removeAll();
```
