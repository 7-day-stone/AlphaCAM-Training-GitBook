# Cleaning Up The Template File

This is the first step after importing your files into AlphaCAM. You must change all the lines to fit the layers you use, and delete any you dont need. Then you'll need to create your inside corner radiuses.

## Changing Layers

Once imported, you will see a file similar looking to this one

![Beginning File](../.gitbook/assets/beginningfile.png)

Each color is a different layer and means something different. Usually, red means finished edge, green means flat polish, orange is for seams/miters, dashed white/black is for cabinet lines, and solid white/black is for walls and the sink center line

Begin by hiding all layers. We're going to first delete the lines we dont need

Start by unhiding the layer that the templator's dimensions are in, and delete them all. We will not ever be using the templator's dimensions, they are only for the templator to use to confirm their template is correct on site.

![Deleting Template Dimensions](../.gitbook/assets/deletetemplatedims.gif)

After dimensions are deleted, unhide the gray layer and delete any lines that are in the gray layer.

Once deleted, we can begin defining our construction\(reference\) lines. These lines will not be seen by the machines and will only be used in our cover sheet file. We use reference lines as points of measure, visual guidance, and for placing our CNC toolpaths in when creating our cover sheet file.

First, unhide the dashed black/cabinet line layer, and change `ctrl + h` them all to construction. Then, unhide the solid black/wall layer, and change the sink/cooktop centerlines to construction as well

It should look like this now

![Changing To Construction](../.gitbook/assets/changingtoconst.jpg)

Now we're finished creating reference lines, so now let's define what we want cut out.

Firstly, unhide all of your layers, then hide **just** your construction lines. Now, change `ctrl + h` everything to Geometry. You should now be able to unhide your construction layer and everything should look something like this

![Finalizing Cleanup](../.gitbook/assets/finalizingclean.jpg)

Now is a good time to make sure that all of your lines are joined together, and that there are no common lines. Common lines are multiple lines that are on top of each other and look like a single line because of it. To ensure everything is joined together and that there are no common lines, we'll use the common line removal tool. The common line removal tool can be found in `Geometry -> Special Funtions -> Common Line Removal`

## Creating Inside Corner Radiuses

Next you must place any inside corner radiuses you may need. To do this, you must first know what your seam locations will be. **Finding your seam locations is talked about on the next page**. Once you know your seam locations, fillet `f` any inside corners there may be.

*What are inside corner radiuses? What are outside corner radiuses?*

![Photo Example Showing Inside vs. Outside Corners](../images/insideoutsidecorners.jpg)

In this stage of programming, cleaning up the file, we should only be creating inside corner radiuses, not outside corner radiuses. This is because our seam locations, laminations, and dimensions are all determined by inside corner radiuses. The case is not the same for *most* outside corners. If we wait too long to fillet our inside corners, we'll have to change a bunch of things at once, putting us behind. If we do our outside corners too early, it'll take longer to do all of our dimensions, or they will just come out wrong.

Inside corners where ever there is a finished edge, should always be 2 1/2". They should never be less than that and any less than that is not able to be ran on the CNC. if, however, it is not a finished edge, then your inside corner radiuses will be determined by what material is being used. 

If the material is a natural stone (granite), a corner radius is not required. They can be kept completely square. 
If the material is any kind of quartz (Ceasarstone, Silestone, Optimus, LG Viatera, Cambria, and other brand names) then all inside corners, regardless of where they are, require at least a 3/8" inside corner radius. Even if it's back up against a wall, it needs to be at least 3/8". There is, however, no requirement for outside corner radiuses.
If the material is Corian or LG Hi-macs solid surface, all finished edge inside corner radiuses must be at least 1".