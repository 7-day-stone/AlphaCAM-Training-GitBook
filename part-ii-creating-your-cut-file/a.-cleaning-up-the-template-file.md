# Cleaning Up The Template File

Once imported, you will see a file similar looking to this one

![BEGINNING FILE](http://tanner.havana.software/t0aKpF)

You will then want to change the lines you need to Construction. To access the `change` tool, press `ctrl+h` and select **from** `Old Layer` **to** `Construction`

![Change Tool](http://tanner.havana.software/A0h7UT)

Then you can start selecting lines to change to construction

![changing gif](http://tanner.havana.software/UHFWHg.gif)

Until you are finished selecting what you want

![fully changed](http://tanner.havana.software/v83b2Y)

The lines that you want to include are the outermost lines that represent the edge of the material you're cutting, any [center lines](http://tanner.havana.software/HlWW9S), and any [refence lines](http://tanner.havana.software/6pMufl) you want, like cab lines and Dish Washer edge lines.

Once you've selected all your lines, complete the change by right clicking.

Now they're construction lines. Construction lines are purple lines that are mainly used for referencing something inside the drawing.

Now that your lines are construction, you can hide all layers aside from construction like so

![hide all](http://tanner.havana.software/FKuYX0)

![unhide construction](http://tanner.havana.software/jg7b0o)

Press `M` to use your move tool. Now select all of your changed lines but don't right click yet. Before you start moving anything, unhide all your layers and additionally select any notes/text you want or need, for example:

![move example](http://tanner.havana.software/Opz1Nr)

Now right click and choose your base point for moving what you've selected. You can just left click anywhere to start moving, then move all your selected layers away from the rest of the drawing.

![move to the side](http://tanner.havana.software/QxacV6)

Right click to finalize the movement.

Next you'll want to delete what's left over. You can do that by pressing `D` to bring out your delete tool, selecting everything you didn't move, and right clicking to finalize the delete. It will bring a pop up message as a confirmation for the delete. You can press `ok` to delete, or just press enter.

![delete](http://tanner.havana.software/4m4GzL)

Now use your move tool again, select your whole drawing, and move it to 0,0 \(x: 0, y: 0\)

To move specifically to 0,0 you have to select what you want to move, right click to finalize the selection, left click to select your base point \(can be anywhere\), then at the bottom you'll see [this](http://tanner.havana.software/6WqlZN). You can type in 0 for both of these boxes then press enter to move it to 0,0. Once moved you can press `ctrl + a` to get the screen to move to your drawing's location and zoom it in to fit your screen.

Now is a good time to join your outermost lines together. Press `J` to use your join tool and select all the outer layers of your drawing. It should look like this once you're finished

![join](http://tanner.havana.software/TQxyps)

Once joined, you can easily change\(`ctrl + h`\) the outermost lines to geometry layers, the same way you changed the original layers to Construction lines.

![geometry layered](http://tanner.havana.software/ztnA1A)

Now it's time to offset your finished edges a quarter inch inwards. The reason why you offset them a quarter inch inwards is because that is where the edge of the material will be once the piece has been cut and edged on the CNC machine.

To figure out which lines need to be offset, refer to the print pdf that was supplied to you in the zip file.

Red lines are lines that need a finished edge, and green lines are lines that are going to be flat polished

![FP vs edge line](http://tanner.havana.software/qLzOzO)

To offset a line, press `o` to bring up your offset menu. Under distance, write .25 \(quarter of an inch\) and press Ok. Then click on the line you want to offset, and click in the direction you want to offset in. For finished edges, offset the lines inward, because the material will be cut down from the geometry line a quarter inch when the CNC process is done.

![offsetting lines](http://tanner.havana.software/wsW1ZE)

Once you have all of your edge lines offset a quarter inch inward, fillet those lines together with a 0 radius.

To fillet lines means to connect them together with a radius. If the radius is 0 then there will not be any curve in the line. Then will go straight until the two lines connect.

to use your fillet tool, press `f` and type in `0` under the fillet radius to make the lines you're connecting stay straight.

![fillet 0 menu](http://tanner.havana.software/dqGHob)

Then click the edges of each line to connect them

![connecting with fillet](http://tanner.havana.software/QpyLwz.gif)

once all these lines are joined together your file is all cleaned up and ready for the next steps.

Before you move on, however, you should save your file here. press `ctrl + s` to save, and the prompt will ask you if you want to override the current file. Hit `No`. This will pull a Window up asking you for a save location and file name. Name the file name the address or job title \(123 MAIN ST\) then save that file inside the job folder.

