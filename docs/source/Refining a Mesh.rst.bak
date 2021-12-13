Refining a Mesh
===============

Reasons to Refine
^^^^^^^^^^^^^^^^^

As mentioned in the initial meshing section, to attain better and more accurate results we can choose to further refine the 
mesh where necessary. Refining the mesh is an important step in any study and can take repeated iterations to complete. 
However, refining the mesh based on study results can lead to much more accurate final results as you will understand from 
your initial results where areas of interest on your model may be. 

Sharp Internal Corner
^^^^^^^^^^^^^^^^^^^^^

One example of a reason to refine one's mesh would be that in some models (depending on how a load is applied) stress can 
appear to be greatest at sharp corners on a model to the point where a area in SOLIDWORKS can appear to be astronomically 
high and show as a stress hotspot as seen in the example image below. This can be the result of a sharp internal corner, 
where stress levels will be a numerical value instead of infinite at the corner due to how FEA analyzes models. This does 
not necessarily mean that stress in this area is actually higher, it just indicates that the mesh is undergoing a higher 
amount of deformation in that area due to the geometry.

.. figure:: ../_static/images/Refining a Mesh 1.PNG
    :figwidth: 600px
    :target: ../_static/images/Refining a Mesh 1.PNG 

Due to the internal sharp corner, stress will continue to diverge the smaller the mesh gets (stress increases as the mesh
quality increases). To compensate for this, it's recommended that a fillet on any such sharp corners be added, regardless of 
what size you choose to make it. To eliminate this possibility we will add 0.025 inch fillet to get rid of this potential 
effect.

.. figure:: ../_static/images/Refining a Mesh 2.PNG
    :figwidth: 600px
    :target: ../_static/images/Refining a Mesh 2.PNG  

Adding Refined Meshes in Specific Locations
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

However with the mesh rebuilt we get the mesh with a new issue, as now there is only a single row of mesh elements that are 
on the new fillet.

.. figure:: ../_static/images/Refining a Mesh 3.PNG
    :figwidth: 600px
    :target: ../_static/images/Refining a Mesh 3.PNG  
 
Only having a single row of elements on the fillet could lead to some inaccuracies in our results, so increasing the number 
of elements on the fillet will fix this issue. This can be done by selecting “Apply Mesh Control '' in mesh options and 
applying a finer mesh (of your choosing) to the fillet as shown below. 
  
.. figure:: ../_static/images/Refining a Mesh 4.PNG
    :figwidth: 600px
    :target: ../_static/images/Refining a Mesh 4.PNG  
 
.. figure:: ../_static/images/Refining a Mesh 5.PNG
    :figwidth: 600px
    :target: ../_static/images/Refining a Mesh 5.PNG  

As well, a finer mesh should also be considered in areas of importance on a model. In the case of the bracket, the bolt 
holes and the mounting hole will be our areas of interest since they’ll be fixtures or experiencing the load in some form.
Therefore, we will also apply the same finer mesh to these areas. 

.. figure:: ../_static/images/Refining a Mesh 6.PNG
    :figwidth: 600px
    :target: ../_static/images/Refining a Mesh 6.PNG  
 
Hitting OK, we should see a finer mesh at the fillet now compared to the rest of the part, giving the final mesh as shown 
below. With these adjustments, your model overall should see a significant improvement in result quality and accuracy. An 
important final note is that whenever any change is made to the model mesh, the model will have to be re-meshed in order to 
apply the changes by just reselecting “Create Mesh” and reapplying the mesh with your previously selected or desired mesh 
quality settings. 

.. figure:: ../_static/images/Refining a Mesh 7.PNG
    :figwidth: 600px
    :target: ../_static/images/Refining a Mesh 7.PNG   
 
We can now re-run the study to obtain new results with much more accurate stress distribution readings:

.. figure:: ../_static/images/Refining a Mesh 8.PNG
    :figwidth: 600px
    :target: ../_static/images/Refining a Mesh 8.PNG  
 
