# Guides

## How can I execute some code?

You can execute code inside the game by opening you chat (usually typing `T` or `/`) and writing `/js 1 + 1`. Well, the `1 + 1` you shoul replace with your code.

## Building stuff

To build things you have to place blocks in the world, right? There is a command for placing blocks in the world called `box()`. This command is a *function* and will place a block exacly where your player is pointing in the world.

But `box()` by itself doesn't know which kind of block you want to place, so you have to put the type between the `()`, for example:

`/js box( blocks.oak )`
`/js box( blocks.stone )`
`/js box( blocks.diamond )`

You can use the name or the number, for example:

`/js box( blocks.oak )` is the same as `/js box( 5 )`
`/js box( blocks.stone )` is the same as `/js box( 1 )`
`/js box( blocks.diamond )` is the same as `/js box( 57 )`

If you want to see all the block types, check [this link](https://github.com/walterhiggins/ScriptCraft/blob/master/src/main/js/modules/blocks.js) or follow this image:

![](https://github.com/walterhiggins/ScriptCraft/raw/master/docs/img/ypgpm_datavalues.png)

## Building bigger stuff

It will take *forever* to build a castle by typing `box( blocks.stone )` block by block but we can use code to build HUGE stuff very quick by using more **parameters** to the **function** `box()`. The way you use it is like:

`/js box( blocks.sand, 3, 2, 1 )`  creates a block of sand 3 wide x 2 high x 1 long
`/js box( blocks.wool.green, 2 )` creates a block of green wool 2 blocks wide

The main idea is to use `box( block, width, height, depth )`, replacing `block` for your favorite block type and `width`, `height` and `depth` by the dimensions of your building. This image can help you to understand this:

![](https://github.com/walterhiggins/ScriptCraft/raw/master/docs/img/ypgpm_whd.jpg)

## Building different stuff

You can build this things with code:

![](https://github.com/walterhiggins/ScriptCraft/raw/master/docs/img/ypgpm_3dshapes.jpg)

`/js box0( block, width, height, depth )` creates an empty box (with the insides hollowed out - perfect for dwellings. box0 will remove both the floor and ceiling too.
`/js cylinder( block, radius, height )` creates cylinders, perfect for Chimneys.
`/js cylinder0( block, radius, height )` creates empty cylinders - perfect for Towers. cylinder0 will remove both the floor and ceiling too.
`/js prism( block, width, depth )` creates a Prism - good for roofs.
`/js prism0( block, width, depth )` creates an empty prism.

## The Drone object

The `Drone` is an (invsible) object you create every time you execute any of the building or movement functions. When you execute...

'/js box(5,3,2,4)'

... a new `Drone` object is created and does the work of building on your behalf. Think of a `Drone` as something like a remote control plane that can move about freely and build things for you. Moving the Drone is easy...

`up( numberOfBlocks )` - moves the Drone Up. For example: up() will move the Drone 1 block up. You can tell it how many blocks to move if you want it to move more than one block.
`down( numberOfBlocks )` - moves the Drone Down.
`left( numberOfBlocks )` - moves the Drone Left.
`right( numberOfBlocs )` - moves the Drone Right.
`fwd( numberOfBlocs )` - moves the Drone Forward (away from the player).
`back( numberOfBlocs )` - moves the Drone Back (towards the player)
`turn( numberOfTurns )` - Turns the Drone Clock-wise (right). For example: turn() will make the Drone turn right 90 degrees. turn(2) will make the Drone turn twice so that it is facing in the opposite direction.

You can make a Drone move around before and after building by daisy-chaining the building and movement functions together. In the game, point at the ground then type the following...

`/js up(1).box( blocks.oak ).fwd(3).box( blocks.oak )`

![](https://github.com/walterhiggins/ScriptCraft/raw/master/docs/img/ypgpm_2boxes.png)