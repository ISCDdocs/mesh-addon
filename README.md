# ISCD blender addon
An addon for blender to interact with [ASCII .mesh files](https://www.ljll.math.upmc.fr/frey/logiciels/Docmedit.dir/Docmedit.html#SECTION00031000000000000000)

## Installation
You will need to have a working version of blender (>2.77) on a linux or MacOs system, available for download on [this page](https://www.blender.org/download/).

To install, download the [iscd.zip archive](https://github.com/loicNorgeot/mesh-addon/releases/download/1.0/iscd.zip), and [install this file as an addon](https://docs.blender.org/manual/en/dev/preferences/addons.html) (File -> User preferences -> Addons -> Install from file).

In order to use the FDS import, you will need to have an active version of python3 on your system, and install the python3 (to use with blender bundled python) [vtk module](https://lorensen.github.io/VTKExamples/site/Python/) module:
```
pip3 install vtk
```

## Utilisation
