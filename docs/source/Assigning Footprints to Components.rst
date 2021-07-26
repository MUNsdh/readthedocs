2 - Assigning Footprints to Components
==================================
.. |assignPCB| image:: ../_static/images/footprint4.png
   :width: 3%
   
.. |filterbys| image:: ../_static/images/footprint6.PNG
   :width: 3%
   
.. |filterbyf| image:: ../_static/images/footprint7.PNG
   :width: 3%
   
.. |filterbyl| image:: ../_static/images/footprint8.PNG
   :width: 3%
   
.. |filterbyn| image:: ../_static/images/footprint9.PNG
   :width: 3%
   
.. |vfootprint| image:: ../_static/images/footprint10.png
   :width: 3%

Understanding PCB Footprints
----------------------------
A footprint is the arrangement of soldering pads for each component. They define the location of how and where the component will be soldered to the board. A component can either be surface mount or through hole as discussed in

Through hole components (THT)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
The yellow section in the figure below is known as the pads - it is the exposed region of metal and the most important part of the footprint as it is where the leads will be soldered to and how the component will be electrically connected. The regions highlighted green on the footprint are going to be printed on the silk screen i.e. they will be visible on the circuit board. The circuit board layers in KiCAD were learnt in :ref:`PCB Layers`.

.. figure:: ../_static/images/footprint1.png
    :figwidth: 700px
    :target: ../_static/images/footprint1.png

THT Capacitor being mounted on a board and the capacitor footprint on kiCad

Surface mount devices (SMD)
^^^^^^^^^^^^^^^^^^^^^^^^^^^
The pads are the red sections i.e. copper layer. It is clear that the pads are not holes like THT but are simply on the copper layer of the circuit board. The grey outline is the component outline on the F.Fab layer, which is useful for board manufacturing houses like `JLCPCB <https://jlcpcb.com/VGR?gclid=CjwKCAjwuvmHBhAxEiwAWAYj-ITIlLQRA1Wo_996nJWkou_tb6e5x8ydLtVoxVGrIuntaySqb4OLfxoC6dwQAvD_BwE>.

.. figure:: ../_static/images/footprint2.PNG
    :figwidth: 700px
    :target: ../_static/images/footprint2.PNG
SMD integrated circuit being mounted on a board and the footprint on kiCAD

Understanding PCB pads
----------------------

Through hole components (THT)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
For through hole pads, the radius of the external circle is the pad size and the radius of the internal circle is the drill size i.e. the size / width of the component lead. The drill size is specified on the data sheet and the pad size is usually estimated as (2*0.38mm + drill size + 0.25mm)

.. figure:: ../_static/images/footprint3.png
    :figwidth: 700px
    :target: ../_static/images/footprint3.png
A THT PCB pad

Surface mount devices (SMD)
^^^^^^^^^^^^^^^^^^^^^^^^^^^
SMD components are simply placed on the pads, unlike THT components that are soldered through the pads. As a result, SMD pad dimensions are simpler and correspond with the component’s lead dimensions.

.. figure:: ../_static/images/footprint2.PNG
    :figwidth: 700px
    :target: ../_static/images/footprint2.PNG
SMD integrated circuit being mounted on a board and its footprint in kiCAD

Selecting footprints
--------------------

Through hole components (THT) and Surface mount devices (SMD)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
1. **Pitch:** the distance between each pin of the component

#. **Body size / shape:** components come in different sizes and shapes (from rectangles, squares, to octagons). There are standardized metric sizes for resistors, capacitors, and inductors but they do not always apply as some inductors are still produced in non-standardized sizes.

#. **Lead size:** the width of the component’s lead, will it fit in the hole?

#. **Component orientation:** Is it radial or axial, vertical or horizontal?

How to Filter Footprints
^^^^^^^^^^^^^^^^^^^^^^^^^^^
Select the assign PCB footprints to schematic symbols icon |assignPCB| on the top toolbar. An ‘assign footprint’ tab should open. There are four footprint filters; 

* |filterbys| - schematic symbol footprint filter to filter based on the component’s reference
* |filterbyf| - to filter footprint list by pin count
* |filterbyl| - to filter by library
* |filterbyn| - to filter by searching name

To assign a footprint, double clicking on the footprint in the filtered footprint tab.
To view a footprint, select the footprint then click on the view footprint icon |vfootprint| on the top right corner of the assign footprints tab.

It is best practice to start by filtering only by schematic symbol footprint filter |filterbys| and then adjust as needed.

Examples: Footprint Selection
----------------------

Through hole components (THT)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^


Surface mount devices (SMD)
^^^^^^^^^^^^^^^^^^^^^^^^^^^
