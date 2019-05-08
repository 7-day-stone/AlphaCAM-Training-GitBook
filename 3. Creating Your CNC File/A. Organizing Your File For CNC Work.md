Now that you've finished your cut file and are ready to mov onto the CNC machine file, you must delete any unnecessary things from the cut file. 

The things you should delete are things like
* Notes that don't pertain to the CNC (Field Notes, Sink Model Text)
* Laminations
* Backsplashes
* Dimensions
* Cutting Boards
* Sign Off Sheet
* Sink and Splash info on Job Title

![Unnecessary Object Removal](http://tanner.havana.software/nhPu4D)

Now separate each piece from each other and arrange them in a straight line, like so

![Arrange Pieces in a straight line](http://tanner.havana.software/oBbtY1)

Now that they're arranged in a straight line, it's time to mirror them. Before mirroring them, create a new line of text by pressing `ctrl + e` and then write the word "mirrored". Once the word mirrored is positioned above the pieces, press `ctrl + h` and change the "mirrored" text to a construction layer.

![Correctly placing the "mirrored" construction layer](http://tanner.havana.software/NQvuUy)

Now we're going to mirror everything. To do this, press `i` and select everything, then go off to the side, press `f3` to enable ortho-mode, and click, draw a straight line down at any length, and click again to finalize the command. Do not keep the original copy. It's **important** that you press f3 when mirroring. This will keep the orientations of the objects exact. Press f3 again after the command to disable ortho mode.

![Mirroring everything](http://tanner.havana.software/auDLwF.gif)


Now we have to insert our CNC table template. To do this, go to the `titan` tab in Alphacam. Under this tab, you will see a button that says `machine profile select`.
This is where we will select one of our CNC machines. Which CNC machine you choose depends on two things. 
1. Which CNC machine the last job used. 
    * We want to be efficient so if we can, keep alternating the jobs between machines 1 and 2. First job machine 1 if possible, second job on machine 2 if possible.
2. Which tools the CNC will need.
    * Your selection can depend on what tools that CNC machine has.
        * Titan 1 has more 4cm tools
        * Titan 2 has more 3cm tools

![Machine Profile Select](http://tanner.havana.software/XICmAk)

![Insert Table Template](http://tanner.havana.software/pwxozP)

You now should move your piece over to the table template that it implemented

![Moved to table template](http://tanner.havana.software/9s0qlN)


Now that your pieces are moved, it's time to orient them the correct way.

Our goal here is to orient the pieces in a way so that the most finished edges possible are facing the machine operator.

To rotate a piece, press `ctrl + r` and then select a piece, right click to finish selection, left click to get a base point (Put this near the piece), then you should be able to rotate it however you want. Only rotate objects by typing the angle in at the bottom where the tool asks for it

![Rotation Angle Prompt](http://tanner.havana.software/NS9DjP)

You will mostly be rotating things 90, 180, and 270 degrees.

Your CNC file should now look similar to this

![Laid Out Properly Facing The Operator](http://tanner.havana.software/YDwc2X)

Now it's time to set our geometry layers to material. Press `s` to set materials. This menu will pop up

![Material menu](http://tanner.havana.software/qbxCPC)

Now, depending on the thickness of your slabs, you need to change the `Material Top: Z`. 3cm material is `1.3` and 4cm material is `1.6`
Set every geometry layer to a material layer now. it should look like this

![Material Layers](http://tanner.havana.software/spJ5X3)

Now that we have our material layers, we're going to change our quarter inch inward offsets to geometry layers

It should be looking Similar to this now

![Construction To Geometry](http://tanner.havana.software/5vGuPB)

Now that we have our cutting lines, it's time to extend them out one inch on each side. To extend something, press `ctrl+ e` and type `1` under the Distance box. Now click on each cutting line's end point to extend it out one inch, just like below, with every cutting line

![Extending our cutting lines](http://tanner.havana.software/ulxft9)