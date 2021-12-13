SOLIDWORKS Modelling 3D Printed Materials
=========================================
It should be noted that representing the material properties of a 3D printed material is extremely difficult to do. For one, 
there are many printing settings & parameters such as infill density, printing orientation or even the type of printer 
being used to print can have an effect on the print & print material. These settings have no real way of being represented 
in SOLIDWORKS since models in SOLIDWORKS are treated as being solid, which may not be the case for the printer parameters. 
As well, SOLIDWORKS does not have any way of properly representing stress within a material since materials applied in 
SOLIDWORKS are treated as homogeneous materials.

As previously mentioned, when a material’s experiences compression that exceeds the material’s flexural strength it will 
fail due to buckling and when a material’s ultimate tensile strength is exceeded the part will experience tension and will 
fail due to shear. If a material is considered “homogeneous”, that means the part is materialistically ideal and its 
flexural strength and ultimate tensile strength are equal. However, 3D printed materials have stress values that are axially 
independent of one another and can vary along a different axis. In SOLIDWORKS the way that material properties are 
configured only considers materials to be homogeneous, meaning that the program does a poor job of accounting for unideal 
materials. It is cautioned that for model analyses with 3D printed models be only used as a rough benchmark for the model’s 
expected performance as all of these mentioned factors can lead to discrepancies from what’s calculated in an analysis 
result. 

Analysis of 3D Printed Materials (Tensile vs. Flexural Strength)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
As mentioned before, flexural strength is a stress value that we will also be including in our simulation, particularly for 
the bending analysis. However as discussed earlier, because SOLIDWORKS can only work effectively with homogeneous materials 
when our model is actually heterogeneous we will have to manually replace the tensile strength value with the flexural 
strength value when completing the bending analysis.
 




