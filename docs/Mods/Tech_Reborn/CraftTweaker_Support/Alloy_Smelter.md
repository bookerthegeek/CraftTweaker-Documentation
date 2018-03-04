# Alloy Smelter
You can call the AlloySmelter package using `mods.techreborn.alloySmelter`

Addition
------
```java
mods.techreborn.alloySmelter.addRecipe(Output, Input #1, Input #2, Ticks, EU per Tick)

mods.techreborn.alloySmelter.addRecipe(<minecraft:gold_block>, <minecraft:sand>, <minecraft:gold_ore>, 40, 500);
mods.techreborn.alloySmelter.addRecipe(<minecraft:iron_block>, <minecraft:sand> * 3, <minecraft:iron_ore>, 40, 500);
```

Removal
------
```java
mods.techreborn.alloySmelter.removeInputRecipe(Input)

mods.techreborn.alloySmelter.removeInputRecipe(<techreborn:ingot:4>);
mods.techreborn.alloySmelter.removeInputRecipe(<ore:dustCopper>);
```

```java
mods.techreborn.alloySmelter.removeRecipe(output)

mods.techreborn.alloySmelter.removeRecipe(<techreborn:ingot:5>);
```

Remove All Recipes
------
```java
mods.techreborn.alloySmelter.removeAll();
```
