# TOSSE
An Efficient 51 lines Matlab code for topology optimization.

TOSSE (Topology Optimization Same Size Elements) is a Matlab code for 2D and 3D topology design problems. 
The code uses the classic 88 lines code known as TOP88 as basis in order to develop an hard 0-1 evolutionary algorithm that, at every iteration, hard kills the elements. The new code is comprised of 51 lines without sacrificing any readability, making it useful for practitioners who want to approach the field.

The algorithm shows an efficiency on averange superior to TOP88 and structures with almost none checkered board patterns.

For more details on the theory and the numerical results you can check the paper available on:
%%%%%%%%

## Usage
On this project three codes are available: 
```
tosse.m
tosse_cant.m
tosse3d.m
```
The first is a topology optimization code for the Messerschmitt-Bolkow-Blohm (MBB) beam. The code can be launched by typing in the Matlab terminal the following command:
```
tosse(nelx,nely,volfrac,mu)
```
where ```nelx``` is the number of elements on the x-axis, ```nely``` is the number of elements on the y axis, ```volfrac``` is the desired volume in the final design and ```mu``` is the volume reduction parameter.

A practical example of a call is:
```
tosse(180,60,0.5,0.97)
```
For a 180X60 design domain with half of the original volume.

