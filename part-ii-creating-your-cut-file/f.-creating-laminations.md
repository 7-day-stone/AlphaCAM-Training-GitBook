# Creating Laminations

To start creating laminations, you must first select the Saber machine profile, under the `machine profile select` tab

![Saber Machine Profile](http://tanner.havana.software/5SVkai)

Once you have it selected, you can use the `backsplash` tool. This tool is what we use to create laminations. Once you open this tool, you will see a menu that lets you edit your backsplash properties. The tool is made for making backsplashes, yes, but the functionality for creating laminations exists within this as well. To create a simple lamination, just click on a geometry finished edge to make a lamination. Normal laminations are to be 1.5 inches in height, and should not have any oversize length.

![Creating a normal lamination](http://tanner.havana.software/KZZGLk)

Though not all laminations are created the same. For euroseams, you will need to add a 2.5 inch oversize, to account for the seam

![2.5 inch oversize for euroseam lams](http://tanner.havana.software/Ny0uoG)

If the angle of connecting finished edges is greater than 90 degree then you must add a 2 inch oversize to the laminations. Otherwise the laminations wont be long enough and will leave a gap where the edges meet.

![2 inch oversize for obtuse angles](http://tanner.havana.software/6E4BB9)

Now you will need to do your inside radiuses before laminations. With this being said, you cant use the backsplash tool on inside radiuses. You need to make custom laminations. In order to create these custom laminations, you need to start by copying the geometry over somewhere else.

![Copying the geometry](http://tanner.havana.software/J7ZLMl)

Offset the Geometry 1.5 inches inward.

![1.5 Inch offset](http://tanner.havana.software/WDFrdg)

Fillet the offset lines 0 so the shape begins to look like this

![Fillet tool](http://tanner.havana.software/n33Yek)

![General Shape](http://tanner.havana.software/bJDpej)

Once it looks like this, you can now make your custom lamination. Press `l` for the line tool, then press `f6` to select the ending of the radius, then press f11 and make a perpendicular line going through the piece. Then move this line a little bit passed the endpoint of the radius. Do this for both sides if you have to

![Making line through lamination](http://tanner.havana.software/o97DPV.gif)

Next select your trim tool `t` and then select every line. And then click all lines you dont need. The ones you dont need are any lines that extend over the lines you made, and the parts of the lines you made that extend passed the geometry lines.

![Timming lines](http://tanner.havana.software/wrt8zc.gif)

Once trimmed, go ahead and join all of these lines together.

If one size of the L shape is really short, you can include that part into the custom lamination, to cut down on an unneeded seam.

![Extended custom lamination](http://tanner.havana.software/AmzVNO)

