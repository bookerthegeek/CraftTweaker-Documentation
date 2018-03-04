# Alloy Smelter

TechReborn allows you to `Add` and `Remove` Alloy Smelter recipes. 

## Recipes

### Removal

There are 2 ways to remove Alloy Smelter recipes, being:

```java
mods.techreborn.alloySmelter.removeInputRecipe(IIngredient);
```

And

```java
mods.techreborn.alloySmelter.removeRecipe(IItemStack);
```
There also is a third way of removing Alloy Smelter recipes, though this one will remove ALL Alloy Smelter recipes registered in the game.

```java
mods.techreborn.alloySmelter.removeAll();
```

### Addition

There is 1 commands for adding Alloy Smelter recipes:

```java
mods.techreborn.alloySmelter.addRecipe(IItemStack,IIngredient,IIngredient,Integer,Integer);
```


## Examples

### Removal

This will remove all Furnace recipes that outputs `<minecraft:glass>`.

```java
furnace.remove(<minecraft:glass>);
```

This will remove all Furnace recipes `<minecraft:quartz>` that use `<minecraft:quartz_ore>` as an input.

```java
furnace.remove(<minecraft:quartz>, <minecraft:quartz_ore>);
```

### Addition

This will add a Furnace recipe that will output a `<minecraft:golden_apple>` when a `<minecraft:apple>` is smelted.

```java
furnace.addRecipe(<minecraft:golden_apple>, <minecraft:apple>);
```

This will add a Furnace recipe that will output a `<minecraft:speckled_melon>` when a `<minecraft:melon>` is smelted and will give the player 1500 xp points.

```java
furnace.addRecipe(<minecraft:speckled_melon>, <minecraft:melon>, 1500);
```

### Fuel

This will set the Fuel value of `<minecraft:rotten_flesh>` to `100`.

```java
furnace.setFuel(<minecraft:rotten_flesh>, 100);
```



## Other Functionality
### Getting all registered Furnace Recipes
```
furnace.all;
```
Returns a [`List<IFurnaceRecipe>`](IFurnaceRecipe).
