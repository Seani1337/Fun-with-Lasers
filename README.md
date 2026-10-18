_**This is a small minecraft map, without any content beside the laser.**_

### **If you don´t care about the way it works:** 
you find most commands under the map. To start the Laser, just press the button. This will activate the process.


### **How the Laser works:**

The Laser is rooted to an armor stand with the "ls" (laser start) tag.
It´ll only be spawned when this armor stand exists.

The command blocks react when the player "#1" in scoreboard "laser" has "1".
When it has 1, the armor stand laser, which basically is the laser (who could´ve guessed that), gets spawned at and rotated in the same direction as the "ls" armor stand. 

Beside some sounds, the scoreboard will now count higher and all the other commands for moving the "laser" when player "#1" has "2" or more will start. 

They tp the armor stand "laser" forward, when their own block (where the armor stand stays) is "red_glazed_glass". 

When the laser moves, player "#1" gets "1" in scoreboard "blocks". The block-traveled count will also be shown as a actionbar-title, only when the armor stand travels.

In case, the armorstand gets inside "gray_concrete", the commands will add the blocks traveled to all players points, set "#1" in every scoreboard to "0" and kill the armor stand.


### How to set the gray_concrete to something else:


### Problems i´ve encountered:

Armor stand falls through blocks, when they don´t have a block under them.



### The direction changing system:

This system is relying on the same system, i´ve used in moving the laser forward.

Because the lasers stays inside the block, i can have a second command block tower (so it´s little more ordered).

The command blocks will now (again) test for "blackstone_stairs" with the "[facing=west/south/north/west]" data (because they´re only able to test for one direction, i took 4 of them to test for north, south,...). When they find the stairs, they´ll rotate the armor stand accordingly and a following command block without the "facing"-data teleports the armor stand` ^ ^ ^1` (in the direction it´s facing 1 block)
