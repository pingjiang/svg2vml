## Version 1.1.1 ##
> This is a maintenance, bug fixing release.  The following issues were fixed:
  * [Issue   5](https://code.google.com/p/svg2vml/issues/detail?id=5): Add IE 8 compatibility.
  * [Issue   3](https://code.google.com/p/svg2vml/issues/detail?id=3): Fix Non-display of any SVG in SVG capable browsers.
  * [Issue   6](https://code.google.com/p/svg2vml/issues/detail?id=6): Stop all get(stroke-width) from returning stroke-color
> Other changes were made to help resolve these issues, including, but not limited to:
  * Allowing for some attributes to cascade down from a Group to the child elements.
  * Adding multiple stops into linear gradients.

## Version 1.1 ##
  * All supported functionality can now be called using the SVG API rather than the SVG2VML API. The library maps SVG syntax to VML when the browser is Internet Explorer. When the browser supports SVG, the SVG2VML implementation is not used.