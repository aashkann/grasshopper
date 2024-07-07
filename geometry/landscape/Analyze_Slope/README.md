# Gh_Analzye_Slope

![](https://github.com/aashkann/grasshopper/blob/Analyze_Slope_Ali/geometry/landscape/Analyze_Slope/Assets/analyze_slope.jpg)

 This Grasshopper file gets a Brep geometry (with no overhangs) and analyzes the slopes of that geometry based on a grid of probs. It outputs the slope percentages as well as vector and mesh visualizations.

## How to use

### Inputs
#### srf
A NURBS surface to analyze. You can replace it with a Brep component

#### U_count
Number of probe rows.

#### V_count
Number of probe columns. 

#### Vis Distance From The Inpuy Surface
The minimum edge length of the output surfaces. 

### Outputs

#### Probe
Probe points.

#### Vec
Slope direction at each probe.

#### Slope Percentages
Slope Percentages at each probe.

#### Mesh
Colored mesh based on the slope percentages

### Notes
- It won't work with overhangs
- It works with multiple geometeries.
- All visualizations are adjustable

