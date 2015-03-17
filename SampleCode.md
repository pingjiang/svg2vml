## Using svg2vml ##
### New Users ###
Using svg2vml is very simple and requires very little change to your existing pages.

Simply place the svg2vml Javascript file on your website add the following to the top of any HTML file in which you wish to use the SVG DOM.
```
<script src="svg2vml.js"></script>
<script>var vectorModel = new VectorModel();</script>
```
You will have to modify the path to the svg2vml Javascript file if you place it in a different folder to the HTML file.
You will need to place the call to svg2vml above all Javascript code that uses the SVG DOM, preferable place it above all other Javascript.

There should be no modification required to standards compliant code as the normal SVG calls are translated to VML

You may need to verify if your code is using the correct methods to create and use objects.  Some browsers allow the use of "document.createElement" to create SVG objects, when instead you should be using "document.createElementNS" and pass in the correct "http://www.w3.org/2000/svg" Namespace.

The following are a few simple examples of the SVG DOM, with svg2vml translating for VML only Browsers.
  * A HTML DIV element with rounded corners by using a SVG - [Example](ExampleRoundedDiv.md).
  * A selection of SVG shapes with gradients - [Example](ExampleShapesWithGradients.md).
  * SVG line elements - [Example](ExampleLineElement.md).
  * A version of the original SVG logo created by Harvey Rayner - [Example](ExampleSVGLogo.md).



### Existing users ###
If you have been using the version 1.0 "vectorModel" code, there are changes that will be made that will make svg2vml incompatible with your existing code.

Since the current released version (1.1.1) is a maintenance release you can carry on using your existing code.  However, in future releases this object will not exist and you should start making changes now to be able to take advantage of the newer code when version 1.2 is released.

Simply replace any reference of the "vectorModel.createElement(..." variable with "document.createElementNS("http://www.w3.org/2000/svg",...".

eg;
```
	var container = document.getElementById("content");
				
	var mySvg = vectorModel.createElement("svg");
	container.appendChild(mySvg);
	mySvg.setAttribute("version", "1.1");
	var myG = vectorModel.createElement("g");
	mySvg.appendChild(myG);
```

would become

```
	var container = document.getElementById("content");
				
	var mySvg = document.createElementNS("http://www.w3.org/2000/svg","svg");
	container.appendChild(mySvg);
	mySvg.setAttribute("version", "1.1");
	var myG = document.createElementNS("http://www.w3.org/2000/svg","g");
	mySvg.appendChild(myG);
```