## What are the different Graphics types? ##

Most of us are familiar with images held on computers & taken by digital cameras.  These images can be stored in many formats, the most well known being JPEG, PNG, TIFF, BMP and GIF.

All of these image formats, despite having numerous differences in how the image is described, compressed and written to disk, all ultimately describe pixels in the image.

Image formats that describe pixels are known as Raster Graphics.

These images have a fixed width and height which is determined by the number of horizontal and vertical pixels .

Trying to expand the image will result in the image becoming pixelated as each pixel is scaled up and increased in size.  This ultimately will lead to an image appearing blocky due to the fact that each individual pixel becomes more and more noticeable as the image is scaled up.

This effect can be reduced by storing the image with more pixels to start with.  However, you will never eliminate this pixelation and the larger image will have a correspondingly larger file size.  The extra detail and the associated cost in file size and transfer time, being completely wasted if the image is only viewed at a smaller size.

Another problem with Raster Graphics is that an image that is of an acceptable quality when viewed on screen, can be either too small when printed or becomes pixelated or blurred due to the fact that most printers have at a minimum 16 times more pixels as a screen does in the same physical area.

The alternative to storing an image by pixel is by describing the lines and shapes that make up the image.

Image formats that describe shapes and draw lines are known as Vector Graphics.

The major advantage of Vector Graphics is that no matter what size the image is scaled to, nor what device it is being displayed upon, the image will always be as sharp and clear as that device allows.

As the file contains all the required information about the image, the file size will always stay the same no matter what you want to use the image for, or at what scale you wish to use it.

Vector Graphics have the ability to produce very small files that describe images that would consume a much larger amount of disk space if stored as a raster image.  However, it should be noted that vector images are not suited to storing real life images.  Images taken with a camera are raster images in origin (even film cameras effectively store the image by pixel with the chemical grains on the film acting as pixels) and provide too much information to be realistically be translated into a vector image (vectorised).  Vector images are much more suited to graphics created on a computer without any real life image components.

As a Vector Graphics file is a description of how to draw an image, it is much easier to change parts of the image, should you need to, after the file has been produced.  This feature was taken further in SVG by allowing the Web Browser to modify the loaded description of any SVG image embedded in the page by Javascript just like any other part of the HTML page.

This feature allows you to design a web page and have entire elements of graphics inside that page react and interact with the user.  With raster images you are limited to using static image maps.  With SVG you can attach an event to the image or to an element of the image and no mater how the image or that element is manipulated the event will still be triggered by the browser.  With a raster image this simply isn't possible.  Using the canvas element you are able achieve this, however the event detection/image tracking code must be written by the developer of the webpage, running in Javascript, rather than using the browsers native code, which naturally should be faster as this is not an interpreted language such as Javascript.
