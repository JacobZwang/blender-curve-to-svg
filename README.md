## :warning: Currently Under Development
- installation currently not working
- to use, run script manually in Blender script editor and click play

# Blender 2.8 curve to SVG

>Blender add-on for exporting 2d curves to scalable vector graphics

## Install
#### Github
- click `code > Download ZIP`
#### Blender
- `Edit` > `User Prefrences` > `Add-ons` 
- click `Install`
- find and select `curve_to_svg.py`
- enable the `Add-on` by clicking on its checkbox
- for more information see the [Blender Manual](https://docs.blender.org/manual/en/latest/editors/preferences/addons.html)
## Usage
#### Export SVG
- select one or more 2d Curves
- ensure curve it set to 2d not 3d in `properties > curve properties`
- go to `properties menu > object properties > Export SVG`
#### Adjustments
- `scale factor` adjusts how many pixels one blender unit represents
- `precision` adjusts the floating point precision
#### More than one spline
- splines are grouped by their assigned material, so a `g` element contains one `path` for each material index
#### HTML Info
- selected 2d curves convert splines to `path` elements
- each point is mapped to path commands in the `d` attribute
- original points coordinates are preserved
- transform` attributes adjust the elements
