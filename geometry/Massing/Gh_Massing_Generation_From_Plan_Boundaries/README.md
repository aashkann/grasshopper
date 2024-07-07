# Gh_Massing_Generation_From_Plan_Boundaries

![](https://github.com/alitghomi/Gh_Massing_Generation_From_Plan_Boundaries/blob/main/Assets/sample.jpg)

This Grasshopper file generates a massing from given plan boundaries as well as floor-to-floor heights and floor count of each boundary curve. It also returns basic area analysis metrics of the generated massing.

## How to use

### Inputs
#### Plan Boundaries
The boundary curve

#### Starting Elevation
Starting elevation of each boundary curve.

#### Floor to Floor Height
Floor-to-floor height of each boundary curve. 

#### Floor Count
Number of floors of each boundary curve.

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

#### Massing Union
Overall generated massing


### Notes
- You can add as many curves as you want but you need to add them separately and merge them in the merge component. Every curve should have the corresponding inputs like floor count. If the number of curves and corresponding values doesn't match, the last item of the shortest list would apply to the rest. For example, if you have 2 curves and 3 floor-count inputs. the 2nd curve would be reused for the 3rd floor count. It can become confusing so I suggest keep the numbers of the inputs the same. If you have 3 curves, make sure to have 3 floor-to-floor heights and 3 floor-count, etc. even if the values are the same.


