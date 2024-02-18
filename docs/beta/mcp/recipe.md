# Creating a Recipe

How to create a recipe:  

1. Go to CraftingManager.java  
2. In the constructor you should see all of the Minecraft recipes being added  
3. At the end of the constructor right after all of the recipes being added you can add your recipe  
(ex. `this.addRecipe(new ItemStack(Item.example, itemNum), new Object[] {"XX", "##", "X", Block.dirt, "#", Item.diamond});`)

| Method    | Description   |
| :---      | :--           |
| Item.example      | What will be crafted (Can be a block or a item)      |
| itemNum      | How much will be crafted      |
| "X" - "#"      | The symbol of what blocks/items are used in the recipe, can be whatever symbol you want      |