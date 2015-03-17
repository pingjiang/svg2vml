# svg2vml Frequently Asked Questions #

  * How do I use svg2vml?
    * Short answer, You don't! Just add a reference to the "svg2vml.js" into your exising page that already uses SVG (currently limited to inline SVG inserted by Javascript) and svg2vml will translate the SVG to VML.
    * The slightly longer answer can be found over in [Usage & Sample Code](SampleCode.md).

  * But what will happen to the project when IE9 is out as it supports SVG by default!? (asked in a Comment by asfoor10,  Mar 27, 2010)
    * Uptake of IE8 a year after it's release was slow.  Looking at the browser market share at that time, IE8 only had around 20% to 24%, IE6 and IE7 combined at that point had a share of 27% to 30%.  So exactly a year after release IE8 still hadn't overtaken the usage of the two previous versions.  This may be different with IE9 as XP is no longer supported, however it seems likely (on these figures) that IE6/7/8 will be with us for some time.

  * Polyline doesn't work, Help!
    * Polyline isn't officially supported in the current release, both the code that was added as a comment to the Wiki and the development code that had been in the trunk (see [r24](https://code.google.com/p/svg2vml/source/detail?r=24) of svg2vml.js) will provide some polyline support.  We have imported basic polyline functionality into v1.1.1 so that you do not need insert the code yourself.  However, as a rewrite of the svg2vml inner class is about to happen, this feature will not be extended until after the re-written class has at-least equal functionality to the existing 1.1.1 release.