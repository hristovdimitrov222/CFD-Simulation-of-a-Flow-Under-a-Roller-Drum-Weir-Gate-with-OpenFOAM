# OpenFOAM CFD simulation of flow under roller drum gate
The code provided here is supplementary to the master's thesis of Dimitrov, H. (2026). CFD Simulation of a Flow Under a Roller-Drum Weir Gate with OpenFOAM. The code is for the Volume-of-Fluid solver "interfoam" of OpenFOAM. The meshes and simulation setups are separated into "with extension" and "without extension", referring to those with and without a jet-guiding structure. For "without extension" there are subfolders to check the filled setup and the filling one. The meshes for each load case are provided in the folder "mesh".

The code can be altered and shared freely. 
 
# How to use
Download the desired cases for testing from the [inter](inter) folder. Run the following commands:

```
decomposePar
mpirun -np 5 interFoam -parallel
reconstructPar
rm -r processor*
```
Observe the results in a post-processing software.

For further understanding of the boundary conditions and how to set them up, please refer to Thorenz, C. (2024): 'Boundary Conditions for Hydraulic Structures Modelling with OpenFOAM', 10th International Symposium on Hydraulic Structures, Zürich. ISSN 0374-0056 , DOI: https://doi.org/[10.3929/ethz-b-000675949] or [HydBCsForOF](https://github.com/baw-de/HydBCsForOF/tree/v2412).
