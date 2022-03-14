# cad_to_urdf_conversion

## 1

If the CAD Software being used is Fusion 360, then the following repo is best suited to convert the CAD model into URDF.

    https://github.com/yanshil/Fusion2PyBullet

The converted URDF can be easily imported in CoppeliaSim software.

## NOTE:
The following things should be kept in mind for successful conversion

  1. The Bullet_URDF plugin should be included in the Fusion 360 CAD Software.
  2. If done, then the pulgin can be observed in the Add-ins section of Fusion 360.
  3. The created CAD model should have a base link named "base_link" for the conversion to take place.
  4. Once the URDF Files are created, duplicate models are formed in CAD Software. These duplicate file names belong to the actual files and the files with actual names should be deleted.
  5. The URDF Files can be saved in any specified location.
  6. The saved files includes a mesh folder, a python file and URDF file.
  7. The URDF File can be imported into coppeliasim software. Menu->Plugins->URDF Import->Import-> <specify the urdf file>
  8. If the file is not imported properly, then using an URDF editor, go inside the URDF File and specify the "path of the mesh folder" for all the links.
  9. Once done, save the file and repeat step 7
  
 
## 2
  
If the CAD Software being used is not Fusion 360,
  1. Save the CAD Model in a specific format.
  2. Import the same model in Fusion 360 software.
  3. Repeat the above mentioned procedure.
  

## 3

     https://github.com/syuntoku14/fusion2urdf
  
This repo can be used to export urdf from fusion 360 directly.

This repo exports:

  1. .urdf file of CAD model
  2. .launch and .yaml files to simulate the robot model on gazebo
  3. .stl files of the robot model
  

 ## Conversion done for a Fusion 360 CAD File
  
 The above mentioned implementation is done to a model created using Fusion 360 softaware. 
 It is then imported into CoppeliaSim Environment using the URDF File created.
  
  
  
 
 ### CAD File - Fusion 360
  
  ![alt text](https://github.com/vishal-kasyap/cad_to_urdf_conversion/blob/main/fusion360_model.png "Model created in Fusion360")
  
  
  
  
 ### URDF Import - CoppeliaSim  
  
  ![alt text](https://github.com/vishal-kasyap/cad_to_urdf_conversion/blob/main/coppeliasim_model.png "Model Imported in CoppeliaSim Environment")
  
  
