# OpenGLDemo 

## Overview

Implemented a sample program to display flat-shaded triangle, tetrahedron and sphere (with tessellation shaders). 
Also implemented a FPS-style camera and local illumination with the Phong shading model. 

Note: Directory `./var/` contains vertices for the required polyhedral objects. 
Each line denotes a 3D point (x, y, and z coordinates), and each 3 lines denote a triangular facet. 
Note that many points are duplicated as they appear in multiple facets!

## Compile & Run

Execute the following commands in the same directory of this README: 
```bash
mkdir build
cd build
cmake -DMAKE_BUILD_TYPE=Release ..
make 
cd ..
./build/OpenGLDemo3D
```

## Usage

- Press `W`/`S`/`A`/`D`/`UP`/`DOWN`, or drag/scroll the mouse to adjust the camera. 

## Notes

- In this program, the sphere parameters passed into tessellation shaders via shader uniforms. 
  Note how this differs from the "pass-by-vertex-attribute-array" method for the circle example; 
- If this program does not work on your VMWare virtual environment, 
  please try to [disable the 3D acceleration feature](https://kb.vmware.com/s/article/59146). 
