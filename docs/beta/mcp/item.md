# Creating a Item

How to create a item:  

1. Create a new Java File and name it what your item is going to be named (ex. ItemSpear.java)
2. Setup the basic structure of the Item Class as laid out below
```
public class ItemExample extends Item
{
    public ItemFood(int itemId)
    {
        super(itemId);
        maxStackSize = 64;
    }

    public ItemStack onItemRightClick(ItemStack itemstack, World world, EntityPlayer entityplayer)
    {
    }
}
```

You then need to register your item so Minecraft knows about it.
1. Open Item.java and go to the botton of the item declarations  
2. Create a new instance of your item  
(ex. `public static Item example = (new ItemExample(95)).setIconIndex(42));`)

| Method    | Description   |
| :---      | :--           |
| itemId      | The unique ID of the item      |
| setMaxStackSize      | The maximum amount of the item allowed in a stack      |
| setIconCoord      | The coordinates of the item in the players hand      |
| onItemRightClick      | Functionality of the right click on the item      |
| getMaxDamage      | Gets the maximum amount of damage applicable by the item      |
| setMaxDamage      | Sets the maximum amount of damage applicable by the item      |
| getItemName      | Gets the name of the item      |
| setItemName      | Sets the name of the item      |
| hitEntity      | Functionality of what happens on entity hit      |
| hitBlock      | Functionality of what happens on block hit      |
| damageItem      | Removes durability of item by specified amount      |
