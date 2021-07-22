# Converting a STEP file to GDML Tessellated Objects.

The following is a suggested workflow for dealing with STEP file
1. Activate the GDML workbench
2. Create a new file ( FreeCAD | File | New )
This should create a file with the following structure
3. Create a New Part under the World Volume
4. Having selected the Part import the STEP file
You can set the FreeCAD general import Options for STEP to import as one compound object or separate objects.
5. You then need to Tessellate the Objects via following Icons/Commands
> * Tessellate
> * Tessellate via Gmsh
> * Using the Mesh Workbench which has a number of meshing options
>> * Gmsh
>> * NetgenThen converting the Mesh to a Tessellated Object using the Mesh2Tess Command/Icon
5. You can set the objects material either via the properties window or selecting the material before the Tessellation operation
6. When you are happy with the Tessellation you can delete the original STEP object.
7. You need to end up with the following structure
>> World Volume
>> A number of Parts under the World Volume, each Part containing a GDML Tessellated Object
8. You can now export the GDML file by selecting the World Volume and using File | Export and selecting GDML as the file type.  