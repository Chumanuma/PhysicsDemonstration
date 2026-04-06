You can run the project through UE5 launcher

Recreating this is simple for physics demonstrations
Assuming you know basics of UE5 you can begin with just choosing a preset with a few props. Steal a wall away and increase it's size to be the bottom of the container.
Hold ALT while click-holding the movement arrows for quick duplicates and construct your box.
Next create a blueprint class and select Actor. This is for your ball or whatever object you wish to test simple physics with.
On the left in the edit window, add your rigid body mesh to the blueprint and follow this with creating a Physics Material under Physics>>>Physics Material under Right Click in Content Drawer.
Play with the settings of said Physics Material then select it in the edit window for your object blueprint (Gravity on, Enable Physics, 0 friction, etc).
Your objects should fall and bounce freely to stress test their impact.

Create a new blueprint just like your bouncing object blueprint and on the left in edit, add a box collision. In the blueprint map for the box collision, Component Begin Overlap >> PlayerCharacter >> Get Level "Lvl_2"
<img width="736" height="297" alt="image" src="https://github.com/user-attachments/assets/3380c4fe-6d11-406d-8883-f986feffaf09" />
Image example above.

This will transition to your second testing site upon contact

Repeat the same steps but ignoring the initial sphere and level box collision parts.
Your preset should have come with some kind of player character mesh and skeleton for physics and animation.
Use the skeleton for your advanced physics testing by opening the PA_Mannequin (Usually in AnimRig folder) or whatever character in the edit window.
CTRL+A to select all the bones and joints and then enable gravity on the right side (details). Then just to give it extra physics and technically the same bouncy rules as the previous object, apply your Physics Mat as well.
Your two levels should now be complete and hit ALT+P to start running the project to feel the difference between rigid simple physics and advanced physics applications.

A Flowchart of the everything step by step:
<img width="1029" height="814" alt="image" src="https://github.com/user-attachments/assets/58c06bbb-c6a9-47ea-886d-072bf481229b" />

Video Link:

