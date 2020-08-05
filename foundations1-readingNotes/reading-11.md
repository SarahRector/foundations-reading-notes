# article on Chart.js API

* makes easy to look at charts easy to create
* import the script to a new HTML page
* add the canvas element
* add the scrjipt that will retrieve the context tof the canvas to the foo of the body element
* change the data array to match your data
* can use chart.js to create line, bar, pie and many other graphs

# Chart.js docs

* really, this is a good refrence for how to use Chart.js

# Mozilla Canvas API Docs
## Basic Usage
* canvass element looks like an image but the only two attributes are width and height ( in the HTML)
    * also a good idea to include id
* can be styled in CSS like regular elements
* creates a fixed size drawing surface

## Drawing shapes with canvas

* the canvas has a grid, squares are normally 1 square pixel and it's anchored in the top left corner at coordinate (0,0)
* three functions draw rectangles on the canvas
    * ```fillRect(x,y,width, height)``` draws a filled rectangle
    * ```strokeRect(x, y, width, height)``` draws a rectangular outline
    * ```clearRect(x, y, width, height)``` clears the rectangle area makes it transparent
* can also draw paths (list of points connected by segments that can be different shapes, curved or not or of different widths and colors)
* first greate a path using ```beginPath()```
* then use drawing commands to draw the path
    * (path methods?)
* Once you have a path you can stroke of fill the path to render it
* you can move the "pen" without drawing by using moveTo(x, y)
* ```lineTo(x,y)``` draws a line from the current drawing position to the position specified by x and y
* arcs or circles are drawn using the ```arc() and arcTo()``` functions

## Applying styles and colors
* can use ```fillStyle and strokeStyle``` to add color
* can also change transparency with ```globalAlpha = transparencyValue```
* lots of ways to style lines ( so many ways)
* can also style how lines connect with each other
* can create both linear and radial gradients
* can create, import and repeat patterns

## Drawing text

* two methods to render text
    * ```fillText (text, x, y [, maxWidth])``` gills a given text at the (x, y) position
    * ```strokeText(text, x, y [, maxWidth])``` strokes a given text at the (x,y) position
    * can style text in canvas with lots of the same types of things as in CSS