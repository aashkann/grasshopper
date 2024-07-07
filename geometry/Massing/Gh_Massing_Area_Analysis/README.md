# Gh_Massing_Area_Analysis

![](https://github.com/aashkann/grasshopper/blob/Massing-Analysis/geometry/Massing/Gh_Massing_Area_Analysis/Assets/area_analysis.jpg)
![](https://github.com/aashkann/grasshopper/blob/Massing-Analysis/geometry/Massing/Gh_Massing_Area_Analysis/Assets/area_analysis_outputs.png)

This Grasshopper file contours a given massing geometry or a collection of geometries based on a list of floor-to-floor heights and outputs areas, floor heights, etc., as well as floor plan boundaries and massing blocks.

## How to use

### Inputs
#### Massing
Series of Breps as massing

#### Floor to Floor heights
Floor to Floor heights of the given massing.

#### Min Ceiling Height
The minimum acceptable ceiling height. 

### Outputs

#### Floor Count
List of floor indexes.

####Floor Elevations
List of elevations of each floor

#### Floor To Floor Heights
List of the floor-to-floor heights resulting from slicing the massing

#### Areas Per Floor
List of total area of each floor

#### Max Building Height
The maximum building height after slicing.

#### Total Area
The total area of all floors

#### Floor Boundaries
The floor boundary curves 

#### Massing Divided
The floor boundary extrusions


### Notes
- It works with multiple massings however it combines all the metrics. If you need the metrics separately you would need to adjust the code or you can copy and paste the entire thing for each massing.
- If the massing geometry and the given floor-to-floor heights don't match, or there are slopes in the massing, the output floor-to-floor heights would vary depending on the minimum ceiling height and the discrepancies between input massing and floor-to-floor heights.


