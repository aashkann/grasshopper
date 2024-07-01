# Gh_Surface_Subdivision

![](https://github.com/alitghomi/Gh-Surface_Subdivision/blob/main/assets/surface_subdivision.png)

 Grasshopper python component to subdivide a surface based on its curveture. This component subdivides a NURBS surface by evaluating mean curveture on various points and subidividing the surface using its isocurves on the max curveture point. It repetes this process until it meets the defined cretaria.

## How to use

### Inputs
#### srf
A NURBS surface to subdivide.

#### probe_count
Number of divisions on the surface to evaluate curvetrue.

#### tol
The maximum mean curvetrue. 

#### min_edge_length
The minimum edge length of the output surfaces. 

#### max_iterations
The number of subdivision iterations 

### Outputs

#### out
out messages of the python component.

#### remainders
parts that do not meet the max curveture because they have small edges or not enough iterations.

#### final_subdivisions
parts that meet the minimum curvetrue.

### Notes
- Since it uses iso curves to subidivde and measure the minimum edge legth, trimmed surface. In those cases I suggest untrim or shrink-trimmed surface and retrim afterwards
- For the same reason it also won't work with triangular networks. In this case you would need to rebuild the surface in such way that iso curves don't converg to zero.

