Designing Schematics in Eeschema
================================

.. |eeschema| image:: ../_static/images/eeschema.png
   :width: 2%
   
Schematic Design
----------------
A schematic is simply the symbolic representation of the circuit as seen in the figure below. The schematics are designed on a schematic drawing sheet (whose size can be adjusted). 

.. figure:: ../_static/images/schematic1.png
    :figwidth: 700px
    :target: ../_static/images/schematic1.png
A simple schematic

For more complex schematics, all the components cannot fit onto the standard schematic sheet. Multiple schematics on different sheets are needed - which implies that the components cannot be visually connected together as they are not on the same sheet. As such, using a global label will connect the components on different sheets together - this set of multiple sheets connected together is called **hierarchical sheets**.

The V5out global label connects all points connected to it, to each other. The set of hierarchical sheets opens more sheets with more schematics and global labels. Click :ref:`Hierarchical sheets` to find out how to do this **AFTER** going through :ref:`Schematic Creation Process` below.

.. figure:: ../_static/images/schematic2.png
    :figwidth: 800px
    :target: ../_static/images/schematic2.png
Hierarchical sheets with global labels connecting the schematics

Schematic Creation Process
--------------------------
At the end of section 1, you should be able to recreate the schematic below. The buck converter schematic is not present on KiCAD so substitute that component with whatever you feel appropriate.

.. figure:: ../_static/images/schematic3.png
    :figwidth: 800px
    :target: ../_static/images/schematic3.png

Follow these steps to create a simple schematic:
1. **Create a new project:** On the top right corner select file >> new >> project. The top toolbar should now be seen.

.. figure:: ../_static/images/schematic4.png
    :figwidth: 800px
    :target: ../_static/images/schematic4.png
      
2. **Toolbars:** Select the schematic layout editor icon (also known as eeschema) |eeschema|. A page with a schematic drawing sheet and three toolbars (top,left, and right) should pop up. The left toolbar can be used to change your units and some other more advanced settings. We will be focusing on the right toolbar.

.. figure:: ../_static/images/schematic5.png
    :figwidth: 800px
    :target: ../_static/images/schematic5.png
Left toolbar
    
.. figure:: ../_static/images/schematic6.png
    :figwidth: 800px
    :target: ../_static/images/schematic6.png
Right toolbar
    

