# Gh_Basic_Fluid_Sim

![](https://github.com/aashkann/grasshopper/blob/Basic_Fluid_Sim_Ali/geometry/landscape/Basic_Fluid_Sim/Assets/flowSample.gif)

This Grasshopper file does a basic fluid simulation on a given geometry based on gravitational direction (Default: 0,0,-1)

## How to use

### Inputs
#### Brep
A Brep to generate the probe points on

#### Count
Probe count.

#### Factor
The amount of movement in every frame. 

#### Reset Button
Resets the simulation. 

#### Run
Starts and stops the simulation. 

### Outputs

#### CrvOut
Curves representing the flows.

### Notes
- You can change the direction of gravity by changing FV vector of the load component


