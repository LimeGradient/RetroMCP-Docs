# Creating a Block

Creating a block is fairly simple and straightforward  

How to create a block:  
1. Create a new Java File and name it what your block is (ex. BlockAmethyst.java)  
2. Setup the basic structure of a Block Class as laid out below
```
public class BlockExample extends Block {
    public BlockExample(int blockId, int blockArt) {
        super(blockId, blockArt, Material.ground) // The material can be changed
    }

    public int idDropped(int i) {
        return 0; // Change to however much you want it to drop
    }
}
```

Then you need to add the block to the Block.java file, which is also pretty straightforward.  
1. Open Block.java and put a block declaration in the file at the bottom of the rest of the block declarations  
(ex. `public static final Block example = (new BlockExample(92, 1)).setHardness(1.5F).setResistance(10F).setStepSound(soundStoneFootstep);`)  

| Method    | Description   |
| :---      | :--           |
| blockId          | The unique id of the block              |
| blockArt          | The id of the block art              |
| setHardness      | How long to destroy a block      |
| setResistance      | How durable the block is against explosions      |
| setStepSound      | The sound played when you step on the block      |