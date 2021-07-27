Going Beyond
============

Custom Symbols in Symbol Editor
-------------------------------
Creating custom symbols is necessary when the symbols you need cannot be found in the kiCAD library. To do this, a datasheet for the component is needed. For this tutorial, let's use this buck converter as an example.

1. **Create a new library to store the new symbol:** Click the symbol library editor icon  on the top toolbar of eeschema or the project page >> file >> new library. Save the library in your desired location then either select  to save it on kiCAD as a global or a project specific symbol. Global symbols can be accessed from any KiCAD project, while project specific symbols can only be accessed from that particular project.

2. **Create new symbol:** Click the new symbol icon on the top left corner. Select the library created in the previous step and then edit the symbol properties - the default reference designator and the symbol name are the settings that should be changed, leave the rest as default. The designator and the name both appear with the symbol.


The default reference designator is used to identify the component in the schematic. KiCAD uses the reference designators to keep track of common components in your schematic, derailing from the standard reference designators can break your project. Do not guess the designator, use the reference designators standard IEEE 200-1975/ANSI Y32.16-1975 as seen below or by visiting here:



3. **Draw symbol outline:** Use the graphic polygon  or lines  tool to draw the outline of the symbol. Left click on the symbol outline to edit the properties. Select the fill background option to shade the outline of the symbol yellow.


4. **Modify pins:** Add pins to the symbol using the pin tool iconbased on the pin configuration from the datasheet. The thing to remember here is that the convention is to group similar pins together and place the two power pins to the top left and bottom right of the rectangle. 

Based on the pin configuration on the datasheet, pin 1 is named the ground. Ground is a power output even though it is not noted as output ‘O’ in the datasheet. Pin 6 is named VBST and is an output. I/O means input / output. Power pins are usually put under the electrical type power input/output, while regular pins are either input/output.




The positions of the pins do not matter and can be different from what is specified on the datasheet. The most important aspect of the symbool is the pin numbers and names. Do not mix up the names i.e. pin 1 must always be ground. Pin 2 cannot be ground.


Importing Symbols into KiCAD
----------------------------
Most symbols for components can easily be found online from sites like mouser, component search engine, or snapeda. After downloading it off the site, import it into Kicad by opening the symbol editor >> file >> import symbol. If you did not initially create a library, one is needed to store the symbol. Follow step 1 of 7.1 - Custom symbols in the library editor to do this.

Custom Footprints in Footprint Editor
-------------------------------------
Custom footprints are important if you can't find the footprint online. It is also important to know how to create your own footprints as sometimes, footprints found online can be incorrect. Incorrect footprints mess up circuit boards by making the components impossible to mount and also impossible to function. Mysa Thermostats cites wrong footprints as one of the driving factors for why their first thermostat launch was delayed. They are very important.

If your component is not one of the following standard body sizes or is not listed under a manufacturer on KiCAD, a custom footprint is needed.

kiCAD Standard Body Sizes

To do this, a datasheet for the component is needed. For this tutorial, let's use this toggle switch as an example. 
1. **Create a new library to store the new symbol:** Click the footprint library editor icon  on the top toolbar of the project page >> file >> new library. Save the library in your desired location then either select  to save it on kiCAD as a global or a project specific symbol. Global symbols can be accessed from any KiCAD project, while project specific symbols can only be accessed from that particular project.
2. **Create new footprint:** Click the new footprint icon on the top left corner. 

3. **Get component datasheet:** This is an excerpt from the part’s datasheet. We will be working in mm. As indicated in the datasheet, the dimensions in mm are in brackets and the one outside the bracket is inches.



4. **Understand KiCAD coordinates:** KiCAD works in coordinates that are oriented as downwards being positive y and to the right being positive x. Creating an outline for the footprint requires that all dimensions from the datasheet be changed into coordinates. 

5. **Sketch footprint using body coordinates:** Always take the origin to be the middle of the body. Write down the body dimensions to figure out the coordinates of the points at where the body intersects.

6. **Improve the sketch with drill size, pad size, and hole coordinates:** determine the drill size by adding an extra 0.25mm to the drill size indicated on the datasheet. The pad size is (2 x 0.38 mm) + drill size. Then determine all coordinates for the points.

The drill size for non-circular leads is essentially the longest dimension of the lead. The choice is between either 0.76 mm or 1.27 mm, of which 1.27 mm is the correct drill size. With the additional 0.25 mm, the drill size becomes 1.52 mm. 



The pad size is (2 x 0.38 mm) + 1.52 = 2.28 mm

Constrain the holes by adding the pitch of 4.7 mm to determine the hole coordinates.


7. **Input sketch into KiCAD:** transfer the sketch to Kicad by inputting the coordinates. If the coordinates are correct, this step should be swift and easy. Draw the outline using the graphic lines tool and place the pads using the add pad tool  on the right toolbar. You can select the line or pad to edit the properties as shown below.


8. **Indicate location of pin 1:** A line as shown below is usually placed at pin 1 to indicate the orientation of the part for easy assembly. This line can easily be placed using the graphic lines tool .


Importing Footprints into KiCAD
-------------------------------
Most symbols for components can easily be found online from sites like mouser, component search engine, or snapeda. After downloading it off the site, import it into Kicad by opening the footprint editor >> file >> import footprint from KiCAD file. If you did not initially create a library, one is needed to store the footprint. Follow step 1 of :ref:`Custom footprints in Footprint Library` to do this.

Importing digikey libraries into KiCAD
--------------------------------------
Sometimes components can be found in digikey libraries. To import the library into kiCAD; the digikey library must be downloaded onto your computer then imported into KiCAD. 

1. **Get the digikey library from the github repository:** Download the zip file.

Github repository

2. **Update both the symbol and footprint libraries:** Go to preferences in the project page. Select manage symbol libraries / manage footprint libraries. Click the add existing library to table icon  and open the downloaded digikey library >> digikey - symbols, then hold the ctrl and ‘a’ key to select all the files in it. Finish the process by clicking ok. The digikey library should now be added to your Kicad. Repeat the same process for adding the digikey footprint library.



Adding a Logo onto the PCB
--------------------------
Logos can be added to KiCAD by transforming the .png image into a footprint, then adding it to the silk layer of the PCB.

1. **Close KiCAD**
2. **Open the project file**

3. **Image must be in .png format**
4. **Convert graphic to footprint:** Select theBitmap to component converter icon  on the top toolbar of the project page. The resolution determines the size of the graphic when it is converted to a footprint. So adjust as needed.

5. **Store graphic:** save graphic in your preferred location.
6. **Import as footprint into KiCAD:** see 7.22 - Importing footprints into KiCAD.
Place on board: open PCBnew. See 4 - Board layout in PCBNEW for how to open PCBnew. Select the add footprint icon  on the left toolbar of PCBnew and place it on board. The footprint library should open where you can then select the graphic that will be stored in your chosen library.

Common Routing mistakes
----------------------
PCB design beginners ud=usually make the following mistakes. Try to avoid them:

1. **Traces that are too close to through-hole components.**  The circled route is two close to a through-hole component. The DRC will not flag this, but since we solder the through-hole stuff by hand, we need to have ample room for our soldering mistakes not to short circuit the vias. 

2. **Minimize ground loop effects.** Ground loop basically means that there are two or more different paths that the same signal can travel from point A to point B. Ground loops can be a cause of noise in the circuit. So wherever possible we should remove that. They are usually caused by having multiple ground planes on both the top and bottom of the board. The effects can be minimized by using a single bottom ground plane and connecting components to ground mostly through vias to minimize the copper traces that are going to ground. Learn more here.

3. **Copper traces that are too close to the board edge.** I suggest increasing the size of the board so there's more margin with the top edge.


4. **Align resistors that are in a column for better aesthetics.**

5. **Add silk screen with logos and version number as finishing touches.** This was covered in :ref:`Adding a Logo onto the PCB`.
Follow datasheet recommended layout


