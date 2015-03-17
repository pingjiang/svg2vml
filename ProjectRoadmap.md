The current release version is 1.1.1 which is available from the [downloads](http://code.google.com/p/svg2vml/downloads/list) page.

## 1.1: Complete basic functionality ##
  * Make gradient uniform for SVG and VML

## 1.1.`*`: Bug fix versions ##
> ### 1.1.1: Several Issues Resolved ###
    * [Issue   5](https://code.google.com/p/svg2vml/issues/detail?id=5): Add IE 8 compatibility.
    * [Issue   3](https://code.google.com/p/svg2vml/issues/detail?id=3): Fix Non-display of any SVG in SVG capable browsers.
    * [Issue   6](https://code.google.com/p/svg2vml/issues/detail?id=6): Stop all get(stroke-width) from returning stroke-color

## 1.2: Complete basic functionality ##
  * Implement polyline
  * Implement gradients for circles and ellipses
  * Implement self initialisation to provide abstraction between Javascript and HTML.
  * Implement a series of tests to improve/speed up testing of releases.

## Extend basic functionality ##
  * Implement Path
  * Implement Matrix Transforms
  * Attempt to implement as much of the SVG 1.1 DOM as possible in VML.
  * Add DOM parser to read embeded SVG and convert to VML.
  * Re-write svg2vml object to allow for more efficient inheritance of CSS properties.
  * Animation.