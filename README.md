## Description

Generate a gmsh geometric model (.geo), a pumi discrete model (.dmg), and gmsh mesh (.msh) then convert the gmsh mesh into an MDS mesh (.smb) for use with SCOREC/core (aka PUMI).

## Setup and Dependencies

Gmodel: https://github.com/ibaned/gmodel

Gmsh - I suggest using the ONElab software bundle: http://onelab.info/

PUMI: https://github.com/SCOREC/core

## Usage

Edit Makefile and set the path to your gmsh install.  The makefile 
assumes that the PUMI binaries (`split`,`from_gmsh`) are in your `PATH`.

Create the models and meshes by running make; `make`.

## Thanks

Thanks to @bgranzow for the example and @ibaned for gmodel. 

`notch2D.cpp` and `Makefile` are from 

https://github.com/bgranzow/goal/blob/7fa770bf6bfd7c2bc92210610e0c6a8fce2b8804/example/mesh/notch2D/notch2D.cpp

and

https://github.com/bgranzow/goal/blob/7fa770bf6bfd7c2bc92210610e0c6a8fce2b8804/example/mesh/notch2D/Makefile
