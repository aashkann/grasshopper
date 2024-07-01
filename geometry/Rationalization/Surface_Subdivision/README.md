# Gh_Surface_Subdivision

![](https://github.com/aashkann/grasshopper/blob/Surface_Subdivision_Ali/geometry/Rationalization/Surface_Subdivision/Assets/surface_subdivision.png)

 Grasshopper python component to subdivide a surface based on its curvature. This component subdivides a NURBS surface by evaluating mean curvature on various points and subdividing it using its isocurves on the max curvature point. It repeats this process until it meets the defined cretaria.

## How to use

### Inputs
#### srf
A NURBS surface to subdivide.

#### probe_count
The number of divisions on the surface to evaluate curvature.

#### tol
The maximum mean curvature. 

#### min_edge_length
The minimum edge length of the output surfaces. 

#### max_iterations
The number of subdivision iterations 

### Outputs

#### out
out messages of the Python component.

#### remainders
parts that do not meet the max curvature because they have small edges or insufficient iterations.

#### final_subdivisions
parts that meet the minimum curvature.

### Notes
- Since it uses iso curves to subdivide and measure the minimum edge length, trimmed surface. In those cases, I suggest untrim or shrink-trimmed surface and retrim afterward
- For the same reason it also won't work with triangular networks. In this case, you would need to rebuild the surface so that iso curves don't converge to zero.

