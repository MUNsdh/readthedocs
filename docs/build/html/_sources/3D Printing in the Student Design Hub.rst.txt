3D Printing in the Student Design Hub
=====================================

.. figure:: ../_static/images/3DPDG1.PNG
    :figwidth: 700px
    :target: ../_static/images/3DPDG1.PNG

Welcome
-------

Welcome to Memorial University's Student Design Hub! Here you have access to multiple 3D printers where can 
bring your digital designs to life! 


Introduction
------------

3D printing or additive manufacturing is a process in which solid objects are made from a digital file. The 
most widely used technique is Fused Deposition Modeling (FDM) in which material is layered to create 
polymer-based parts, ranging from basic to complex geometrical shapes. These can be standalone parts 
and/or components of a bigger structure. The relative speed of creating these parts (a couple of hours 
depending on size, design, and infill) allows for proof of concepts to be developed rapidly, moving past 3D 
modeling, a very powerful tool tied to 3D printing. The end results used to be used exclusively for 
prototyping, however, due to the advancements of 3D printing technology and materials, 3D prints are 
being used more frequently as end products and parts.

For more detailed information please visit the sources used under Reference List

Materials
^^^^^^^^^

The most common materials for 3D printing are **Poly Lactic Acid (PLA)** and **Acrylonitrile Butadiene
Styrene (ABS)**. PLA filament is a biodegradable material that is easy to print due to its low heating 
requirements, however it does not possess a very high resilience to UV rays, its more suitable for parts 
used indoors and at around room temperature. ABS filament in the other hand requires a higher 
temperature to be printed, but it offers UV resilience as well as better mechanical properties in high 
temperature environments. There are many other materials available to print as well, depending on the 
printer you use. Some materials are:

* Polyethylene Terephthalate Glycol (PETG)
* Thermoplastic Polyurethane (TPU)
* High Impact Polystyrene (HIPS)
* Polycarbonate (PC)
* Thermoplastic Elastomer (TPE)
* Nylon
* Acrylonitrile Styrene Acrylate (ASA)
* Polypropylene (PP)
* Polyvinyl Alcohol (PVA)
* Glass Fiber or Carbon Fiber Infused
* Metal or Wood Fill
* Etc.

Modelling
^^^^^^^^^

One of the advantages of 3D printing is that very complex models can be achieved. However, when 
crafting your 3D model in a computer-aided design (CAD) software, such as SolidWorks, some design 
considerations can help ensure better results.

**Resoultion:** Similar to image resolution, a 3D printer has a minimum feature analogous to a pixel in 
picture, this is the smallest “dot” it can print, and it is dependent on the nozzle size. 
Resolution is divided into XY-resolution, dependent on the nozzle diameter and the smallest movement the 
stepper motor on the printer can achieve and the Z-resolution is dependent on the layer height. 
Each printer can have a different minimum layer height.

 
.. figure:: ../_static/images/3DPDG3.PNG
    :figwidth: 600px
    :target: ../_static/images/3DPDG3.PNG

.. figure:: ../_static/images/3DPDG4.PNG
    :figwidth: 600px
    :target: ../_static/images/3DPDG4.PNG

**Orientation:** Printing orientation of the 3D model can greatly 
improve the surface quality of the print. The figure displays the same 
3D model printed horizontally and vertically. The horizontally print 
would display a “staircase” pattern, while the on vertically print this 
patter would be greatly reduced achieving a smoother print. 
Conversely, when printing parts that would undergo a mechanical 
load, the former would support more force applied to it at the peak of 
the semi-dome than the latter. 

.. figure:: ../_static/images/3DPDG5.PNG
    :figwidth: 600px
    :target: ../_static/images/3DPDG5.PNG

**Size:** If you are making a display model, then this is less critical as you can scale your 
design before printing to be within the boundaries of the printing volume. This is determined 
by the building platform’s area and the height of the printing chamber. Each printer has its 
own unique printing volume.

**Wall Thickness:** A minimum wall thickness is required for the 
model to be able to print and be structurally sound. This dimension 
would be affected if the model needs to support any force, but as a 
rule of thumb for ABS it is recommended to use a minimum wall 
thickness of 1.2mm. Different materials and printers have their own configurations.

**Shrinkage and Assembly:** When printing parts that are design to 
be connected to each other, keep in mind the shrinkage that the 
prints will undergo. This deviation of the print from the model’s 
nominal size is also known as **dimensional accuracy** and is 
generally around 0.1% or ±0.2mm.


.. figure:: ../_static/images/3DPDG6.PNG
    :figwidth: 800px
    :target: ../_static/images/3DPDG6.PNG

**Embossed and Engraved Details:** Engraving refers to details added into the print (inwards), 
a minimum line thickness of 1 mm and a depth of 0.3 mm is recommended. By contrast, embossing 
are details that protrude from the printed model, a line thickness of at minimum 2.5 mm and a 
depth of at least 0.5 mm is advice. Engravings are usually preferred as they require much lower 
tolerances than embossing details.

.. figure:: ../_static/images/3DPDG7.PNG
    :figwidth: 800px
    :target: ../_static/images/3DPDG7.PNG

**Support Material:** To be able to achieve intricate designs most 3D printers employ support 
material. The most popular ones being soluble and breakaway ones. Both types of supports have their 
cons and pros, soluble support materials are easy to remove, since it dissolves on a solution, 
leaving behind a clean print, however some soluble support material such as PVA take up to 24hrs 
to fully dissolve. By contrast, breakaway support materials can be removed from the print as soon 
as the model is completed, but in certain complex geometries they tend to leave residue behind 
and/or are difficult to completely remove without damaging the print if the design possess 
deep channels or crevices in the inside faces of the model, especially if no exit hole is 
built into the design. This is very important to keep in mind when modeling your 3D design.

.. figure:: ../_static/images/3DPDG8.PNG
    :figwidth: 600px
    :target: ../_static/images/3DPDG8.PNG

.. figure:: ../_static/images/3DPDG9.PNG
    :figwidth: 600px
    :target: ../_static/images/3DPDG9.PNG

**Moving Parts:** Support material allows for the printing of preassembled models 
with moving parts, for these to successfully print a minimum clearance of 0.4mm 
is advised, the greater the space that can be afford, the better chance the model has to print properly.

.. figure:: ../_static/images/3DPDG10.PNG
    :figwidth: 700px
    :target: ../_static/images/3DPDG10.PNG

STL Format
^^^^^^^^^^

After you have finished your design, save the SolidWorks model in the native format SolidWorks Part File 
(SLDPRT) as well as the Standard Triangle/Tessellation Language file format (STL) [1]. To save your 
model in STL format go to File>>Save as, and change the file format from SolidWorks Part (*.prt;*.sldprt) 
to STL (*.stl) in the prompted window, as shown in the image below:

.. figure:: ../_static/images/3DPDG11.PNG
    :figwidth: 600px
    :target: ../_static/images/3DPDG11.PNG

The SLDPRT file stores the part as a solid model, keeping the specified details of material, color, and 
texture. On the other hand, an STL file stores only the information of the 3D model surface, it represents 
this surface as small adjacent triangles.

.. figure:: ../_static/images/3DPDG12.PNG
    :figwidth: 700px
    :target: ../_static/images/3DPDG12.PNG

Printing
^^^^^^^^

The .STL file will be imported into a slicer, a software that produces a path for the 3D printer to 
follow to be able to print the model. This set of commands or language is known as G-code, and it 
tells the printer what movements to make from begging to end of the print.

.. figure:: ../_static/images/3DPDG13.PNG
    :figwidth: 700px
    :target: ../_static/images/3DPDG13.PNG

uPrint SE
---------

.. figure:: ../_static/images/3DPDG2.PNG
    :figwidth: 700px
    :target: ../_static/images/3DPDG2.PNG

To have parts printed with the uPrint SE 3D Printer, please visit  :ref:`Requesting Parts From the Digital Design and Prototyping Lab`.

Eryone ER-20
------------

.. figure:: ../_static/images/Eryone1.PNG
    :figwidth: 350px
    :target: ../_static/images/Eryone1.PNG

How to Use the Eryone ER-20 Printer
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

There are a few steps involved before printing with the Eryone ER-20 printer. The first is to 
make sure your 3D model has been saved in STL format. Please review :ref:`STL Format` to learn how. 

The next step is selecting a material to use in this print. The Eryone ER-20 supports 3 different materials:
 
* **Poly Latic Acid (PLA):** PLA filament is a biodegradable material that is easy to print due to its low heating requirements, 
  however it does not possess a very high resilience to UV rays, its more suitable for parts used indoors and at around 
  room temperature.

* **Polyethylene Terephthalate Glycol (PETG):** PETG is a more durable filament then PLA. It has good chemical resistance, 
  flexibility, and impact resistance. As well as being good for clear prints, however this also means “post processing” such 
  as sanding or removing supports can be much more difficult. 

* **Thermoplastic Polyurethane (TPU):** TPU is a rubber like filament offering it flexibility and versatility, however it 
  can be more of a challenge to print. 

More information on each filament can be found `here <https://3dinsider.com/pros-and-cons-3d-printing-filaments/>`_

Once you have chosen a material, the next step is to upload your STL to a Slicer. In this case we will be using Simplify3D. 

There are two guides to using Simplify3D: A quick guide for very easy and simple PLA parts such as a chess piece and a detailed 
guide for more complex parts and different materials. 
 
Open up Simplify3D by double clicking the icon. 

.. figure:: ../_static/images/Eryone2.PNG
    :figwidth: 400px
    :target: ../_static/images/Eryone2.PNG

You should be brought to this page.

.. figure:: ../_static/images/Eryone3.PNG
    :figwidth: 700px
    :target: ../_static/images/Eryone3.PNG


If there is already an item(s) on the screen, please select the “Remove” button. Then click “Import”, this should bring you 
to file explorer where you will open up your STL.

.. figure:: ../_static/images/Eryone4.GIF
    :figwidth: 700px
    :target: ../_static/images/Eryone4.GIF

Here is where you can view your model from different angles. By left clicking and dragging you can rotate around the model, by 
right clicking and dragging you can change the point of rotation. The command bar on the right side of your screen is 
also available for quick changes to different viewing planes, similar to *SOLIDWORKS*.

.. figure:: ../_static/images/Eryone5.PNG
    :figwidth: 500px
    :target: ../_static/images/Eryone5.PNG

This command bar also lets the user position, scale or rotate their model. You can also double click your model for 
precise numerical changes and the ability to reset any changes.

.. figure:: ../_static/images/Eryone6.GIF
    :figwidth: 700px
    :target: ../_static/images/Eryone6.GIF

The center and arrange button will automatically fix the orientation of your part(s) and make them fit on the bed. 

When arranging your part on the bed there is a few things to take into consideration. FDM printing is done by 
layering melted thermoplastic on top of itself, building from the ground up. You can not print something in thin 
air, there needs to be something to support it. Take a look at this bracket:

.. figure:: ../_static/images/Eryone7.PNG
    :figwidth: 700px
    :target: ../_static/images/Eryone7.PNG

The first arrangement does not work because it requires plastic to be laid down in thin air. The second arrangement will 
print however, you should also look at the largest **FLAT** surface of your model and print from there. This will 
assure good bed adhesion and a better chance at a successful print. The third option with a large **FLAT** surface to 
print from and no overhang is the best option for this model. 

Once your part(s) are arranged on the bed, click “Edit Process Settings”. This window should appear:

.. figure:: ../_static/images/Eryone8.PNG
    :figwidth: 700px
    :target: ../_static/images/Eryone8.PNG

This is the command center of Simplify3D, everything happens in here. In this quick guide we will not be going through all 
the settings but instead checking a few things to make sure everything is right before you print. If your model consists of 
any of the following features, then you may want to consider the “Advanced Guide”:

* Non-PLA Material
* Large Overhang (Support structures needed)
* Thin Walls
* Fine Details
* No Large Flat Surface to Start Print From
* Needs to be Especially Dense or Strong
* Multiple Colours or Materials

See here an example sheet.
:download:`pdf <Advanced Guide pdf.pdf>`

*Subject to change*

If your part is simple and does not fall under any of the above categories, then please follow the instructions below.

Once you select edit process settings this page should appear. Make sure everything is in the green boxes matches your 
screen. “Coast at End” and “Wipe Nozzle” should not be checked.

.. figure:: ../_static/images/Eryone9.PNG
    :figwidth: 700px
    :target: ../_static/images/Eryone9.PNG

Now click the layer tab and check these settings:

.. figure:: ../_static/images/Eryone10.PNG
    :figwidth: 700px
    :target: ../_static/images/Eryone10.PNG

Next the Additions Tab, only skirt/brim should be checked. Uncheck any other boxes if they are on. 

.. figure:: ../_static/images/Eryone11.PNG
    :figwidth: 700px
    :target: ../_static/images/Eryone11.PNG

Next is the infill tab. The offset boxes should rarely be touched but if it is not the same, use the add and remove angle 
buttons to navigate the boxes. 

.. figure:: ../_static/images/Eryone12.PNG
    :figwidth: 700px
    :target: ../_static/images/Eryone12.PNG

Nothing should be selected in the support tab.

*Temperature tab to be updated*

Nothing should ever be touched in the G-Code tab, but just to be sure, check these settings:

.. figure:: ../_static/images/Eryone13.PNG
    :figwidth: 700px
    :target: ../_static/images/Eryone13.PNG

In the Scripts tab there are a few different windows. Layer Change, Retraction and Tool Change Scripts should all 
be blank. The Starting and Ending Scripts should look like this.

.. figure:: ../_static/images/Eryone14.PNG
    :figwidth: 700px
    :target: ../_static/images/Eryone14.PNG

.. figure:: ../_static/images/Eryone15.PNG
    :figwidth: 700px
    :target: ../_static/images/Eryone15.PNG

Next is the Speeds tab.

.. figure:: ../_static/images/Eryone16.PNG
    :figwidth: 700px
    :target: ../_static/images/Eryone16.PNG

The Other tab. Filament Properties and Tool Change Retraction does not affect the print.

.. figure:: ../_static/images/Eryone17.PNG
    :figwidth: 700px
    :target: ../_static/images/Eryone17.PNG

*Bridging is subject to change*

And finally, the Advanced tab.

.. figure:: ../_static/images/Eryone18.PNG
    :figwidth: 700px
    :target: ../_static/images/Eryone18.PNG

These should all be the default settings under the “Eryone ER-20” profile however it is always good practice to check and make sure.

.. figure:: ../_static/images/Eryone19.PNG
    :figwidth: 600px
    :target: ../_static/images/Eryone19.PNG

Select the “OK” button, the window should close. Now click “Prepare to Print!”. You should be brought to this screen where 
you can how the model will be printed layer by layer. 

.. figure:: ../_static/images/Eryone20.GIF
    :figwidth: 700px
    :target: ../_static/images/Eryone20.GIF

You can also view the different features that that the print has. 

For a simple print there is nothing needed to do here. In the top left corner Simplify3D estimates the build time 
however, it is rarely accurate. A good practice is to add about 20% more time, but it may be more or less.
 
You now want to acquire the Micro SD card and plug it into the computer using the USB A adapter. Now click “Save 
Toolpaths to Disk” and transfer the SD card to the printer (Via Left side hole).

Make sure the printer is turned on. There is a power switch in the back. As well make sure PLA filament is inserted into 
the hot end with sufficient filament still left on the spool. To learn how to insert filament click “here”.

When the printer is on, this should be the home page. Click the wheel and scroll to the bottom where it says, “Print 
from media”. Select the file you saved to the SD card and select print.

.. figure:: ../_static/images/Eryone27.GIF
    :figwidth: 300px
    :target: ../_static/images/Eryone27.GIF

If everything is okay, your model should print. It is a good idea to check on your print periodically to make sure nothing is 
going wrong. If you need to stop the print for whatever reason, click the button and scroll to “Stop Print”. A Successful print 
looks like this. 

.. figure:: ../_static/images/Eryone21.GIF
    :figwidth: 300px
    :target: ../_static/images/Eryone21.GIF

Once the print is complete, let the bed cool down a little bit then peal your part off the bed. 

Congratulations! Your model should now be printed. 

.. figure:: ../_static/images/Eryone26.PNG
    :figwidth: 350px
    :target: ../_static/images/Eryone26.PNG

Advanced Workflow
^^^^^^^^^^^^^^^^^

Welcome to the Advanced Workflow! Please expand the Eryone ER-20 tree on the left side of your screen to view all sections.

Changing and Inserting Material
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Changing the material with the Eryone printer is a very simple process. The first thing you want to do is find your selected
material and bring it to the printer. 

Now, you want to grab the wire cutters and the end of the filament, being very careful not to let go of the filament so it does 
not flick back to the spool and get tangled up. Cut the end of the filament at a 45° angle and keep hold of the end or place 
it back in the side spool hole.

.. figure:: ../_static/images/Eryone37.PNG
    :figwidth: 500px
    :target: ../_static/images/Eryone37.PNG

If there is no filament in the printer already,
*to be updated*

Large Overhang/ Support Material
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Supports are needed for 3D models that have large overhangs and unsupported areas. When 3D printing with the Eryone ER-20, it is 
best to avoid supports whenever possible. Printers with only 1 extruder are limited to just break-away supports which can lead to 
poor finishes and more post processing. Supports also increase printing time. Sometimes you can reorient your part or even edit 
the design to make it more 3D printing friendly.

.. figure:: ../_static/images/Eryone38.PNG
    :figwidth: 400px
    :target: ../_static/images/Eryone38.PNG

Take this H as an example. If the H were to be printed vertical, supports would be needed to print the middle section. By rotating 
the part on to its back, supports are no longer needed and there is also a larger flat surface to print from which is 
good for bed adhesion. 

That being said, sometimes avoiding supports is not an option and they must be used. Look at these pictures of a bracket. No matter 
what way it is oriented, supports will be needed for a successful print.

.. figure:: ../_static/images/Eryone39.PNG
    :figwidth: 700px
    :target: ../_static/images/Eryone39.PNG

Fortunately, Simplify3D has an automatic support structure system. With a few clicks you can generate automatic supports and even 
customize them to fit your part’s structural needs. 

Arranging your part with supports follows the same rules as normal. Try and find the largest flat surface of your part to print 
from. You also want to orient your part so that little support is needed. The best option for the bracket would be the second 
orientation, a large flat surface to print from and little support.

.. figure:: ../_static/images/Eryone35.PNG
    :figwidth: 400px
    :target: ../_static/images/Eryone35.PNG

Once your part is arranged on the print bed, click the “Customize Support Structures” icon on the command bar to the right.

.. figure:: ../_static/images/Eryone46.PNG
    :figwidth: 400px
    :target: ../_static/images/Eryone46.PNG

This window should appear.

.. figure:: ../_static/images/Eryone41.PNG
    :figwidth: 400px
    :target: ../_static/images/Eryone41.PNG

Select “Generate Automatic Supports”, then select “Done” and view the automatic supports created for your part. 

.. figure:: ../_static/images/Eryone42.PNG
    :figwidth: 400px
    :target: ../_static/images/Eryone42.PNG

Simplify3D generally has pretty good support generation, however some adjustments may need to be made depending on your 
part. In our bracket example there are several holes. Vertical circular holes are usually not an issue for 3D printers, with 
each layer being so small, the printer can just slowly close the gap without supports. However, as you can see above, a support 
has been made for one of the holes.  This is where customizing your supports can come into play. 

Go back to the Customize Support tab and click “Remove existing supports”. Now click the individual red pillars that you 
would like to remove, in our case it is just the support in one of the holes.

.. figure:: ../_static/images/Eryone43.GIF
    :figwidth: 700px
    :target: ../_static/images/Eryone43.GIF

If you want to add support structures, select “Add new support structure” and place as desired. 

.. figure:: ../_static/images/Eryone45.GIF
    :figwidth: 700px
    :target: ../_static/images/Eryone45.GIF

When adding or removing support structures it is important to keep in mind one thing; are the supports necessary? You do no want 
to have excess supports, this will lead to a poorer finish and more post processing. So, when adding supports be careful, Simplify3D’s 
automatic supports should usually be enough. When removing, be careful as well and only remove unnecessary structures 
like the supports in this bracket’s vertical holes. 

Once you are happy with your supports, select “Done” and go to “Edit Process Settings”, then go to the “Support” tab. There 
are 5 boxes we need to go over. 

**Support Material Generation**

If you want to include your supports make sure the “Generate Support Material” box is checked. The “Support Extruder” should always 
be “Extruder 1” because the Eryone ER-20 only has a single extruder. “Support Infill Percentage” should be at 30% and is generally 
a good number unless you are dealing with fine details or small spaces that require support. You can increase this percentage 
but remember the more you increase the percentage the longer your print will take. Next is “Extra Inflation Distance”, this 
will make the supports “wider” depending on how big you set the number. It should be set to 0 however, may be useful if your 
support-needed area is really small and you need some extra space to build your part off of. “Support Base Layers” are a tool 
used to help create a better adhesion to the bed surface. If you are finding that your supports are coming loose from the bed, 
this tool will make the first X number of layers denser without making the entire support that dense to save 
time. *“Combining Support Layers” to be edited.*

**Dense Support**

Extruder 1 should always be selected. “Dense Support Layers” will add X number of layers in between the top of the support 
structure and the bottom of the actual print. This could be a useful tool if you want a larger surface area for the actual print 
to begin while saving time by not having the entire structure that dense. “Dense Infill Percentage” will determine how dense 
those top layers will be. 

**Automatic Placement**

This box only affects the automatic support generation feature and since we have already manually adjusted our supports usually 
do not need to touch anything here. However, it can be useful.

“Support Type” can be Normal or From Build Platform Only. Build platform will insure that supports only start from the bed 
surface and will not be added into things like our bracket’s vertical holes. This can be a quick tool to get rid of any 
unnecessary supports however since we already manually deleted the hole’s support, it does not need to be changed. As well 
sometimes you may need supports that start from a piec of your part.

.. figure:: ../_static/images/Eryone47.PNG
    :figwidth: 450px
    :target: ../_static/images/Eryone47.PNG

*This would not be the recommended orientation for this part but just used as an example.*

“Support Pillar Resolution” is how large the red pillars are. This can be increased to save time adding supports to large areas 
or decreased to add supports in smaller places.  “Max Overhang Angle” should be set at 45°. Changing this will determine where 
automatic support structures will be placed based on the angle of the print. 45° is the general rule of thumb for support 
structures but can be altered if you are having trouble with a smaller angle or do not need supports until a certain angle.
 
To reapply these settings to your automatic support generation feature. Go back to the customize support window, select 
“Clear All Supports” and then “Generate Automatic Supports”.

**Separation From Part**

“Horizontal Offset From Part” should be set at 0.30 mm. This is used to create some distance between the support and a 
vertical wall of your part. You may want to increase this if you find the support structures are interfering with vertical 
walls. 0.30 mm is usually fine. Upper and Lower Vertical Separation layers should be set at 1 and will create a distance between 
the support structure and your part. This makes the support structure easier to remove. If you are having trouble removing 
supports you can increase this number but be careful, increasing this too much may render the supports useless.
 
**Support Infill Angles**

This box will usually just say 0. Adding an angle of 30° (for example) will make the support structure switch back and 
forth between a straight line and a line at 30° for each layer. This tool can be used to create the look of a denser support 
structure, however, is not commonly used.

.. figure:: ../_static/images/Eryone48.PNG
    :figwidth: 450px
    :target: ../_static/images/Eryone48.PNG

To view any of your changes to these settings you can exit the process settings and select “Prepare to print”. This will 
show how your support structures will be printed and you can judge your changes from this section. 

















 








 








Raise3D E2
----------

To be updated. 


