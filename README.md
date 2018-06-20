# ISCD blender addon
An addon for blender to import/export with ASCII [.mesh files](https://www.ljll.math.upmc.fr/frey/logiciels/Docmedit.dir/Docmedit.html#SECTION00031000000000000000) and [FDS](https://pages.nist.gov/fds-smv/) simulation results.

This addon can be used to interact between blender created models (and functionalities!) and softwares such as [mmgtools](http://mmgtools.org), [tetgen](http://wias-berlin.de/software/index.jsp?id=TetGen&lang=1), [metis](http://glaros.dtc.umn.edu/gkhome/metis/metis/overview), [gmsh](http://gmsh.info/), [medit](https://github.com/ISCDtoolbox/Medit) and [other tools](https://github.com/ISCDtoolbox) developed at the [ISCD](http://iscd.upmc.fr).

## Installation
You will need to have a working version of blender (>2.77) on a linux or MacOs system, available for download on [this page](https://www.blender.org/download/).

To install, download the [iscd.zip archive](https://github.com/loicNorgeot/mesh-addon/releases/download/1.0/iscd.zip), and [install this file as an addon](https://docs.blender.org/manual/en/dev/preferences/addons.html) (File -> User preferences -> Addons -> Install from file).

Once installed, the addon operators will be available in the properties panel of blender, on the left side of the 3D view, under the "ISCD" tab.

Note that in order to use the FDS import, you will need to have an active version of python3 on your system, and install the python3 (to use with blender bundled python) [vtk module](https://lorensen.github.io/VTKExamples/site/Python/) module:
```
pip3 install vtk
```

## Basic usage
The following operations are possible from the ISCD tab:
1. **Import a .mesh**: imports a .mesh file in blender.
2. **Export a .mesh**: exports a blender object to a user-specified .mesh file, using objects materials as references.
3. **Import a .mesh sequence**: imports a sequence of .mesh objects - in the format result.x.mesh, x being an integer number - to blender. Use the "morphing" for constant number of triangles, and the "fluidsim" for varying number of triangles.
4. **Import FDS results**: imports results (flame and smoke) from a [FDS](https://pages.nist.gov/fds-smv/) simulation as isosurfaces. Requires a python3 vtk installation.
<p align="center">
<img src="https://user-images.githubusercontent.com/11873158/41673413-27f33548-74bd-11e8-889e-4403ce3fff37.png"/>
</p>

## Advanced usage
Other examples of fluid import/export usage,  can be found on the 2017 summer school [repository](https://github.com/ISCDtoolbox/pythonMesh).
