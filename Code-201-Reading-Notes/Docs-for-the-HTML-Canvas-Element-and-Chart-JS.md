# Docs for the HTML `<canvas>` Element

* `<canvas>` is an HTML element that is used draw graphics with JavaScript scripts.
* Some examples of things we can do with `<canvas>` include:
    - draw graphs
    - combine photos
    - create animations
* By default, the size of the canvas is 300 pixels by 150 pixels. However we can customize the dimensions using width and height attributes.
* To draw on the canvas, we use a JavScript context object that allows us to create graphics.
* To make the canvas easier to identify in a script, we can use the id attribute. For example: <br />

<canvas id="tutorial" width="150" height="150"></canvas>

* The canvas is completely transparent by default, but we can apply styling rules to customize it.
* To get the rendering context and it's drawing functions we use a method of the `<canvas>` element called `getContext()`  For example: <br />

let canvas = document.getElementById('tutorial'); // retrieves the node in the DOM representing the <canvas> element by // calling document.getElementById() method
let ctx = canvas.getContext('2d'); // access the drawing context using its getContext() method.

## Drawing Shapes With Canvas 

* `<canvas>` allows us to make two primitive shapes: rectangles and paths (lists of points connected by lines) but we can make other shapes as well by combining one or more paths.
* There are 3 different functions we can use to draw rectangles
    1. `fillRect(x, y, width, height)` // draws a filled rectangle.
    2. `strokeRect(x, y, width, height)` // draws a rectangle outline.
    3. `clearRect(x, y, width, height)` // clears the specified rectangular area, making it fully transparent.
* Here is an example of drawing a rectangular shape using `<canvas>`: <br />


function draw() {
  var canvas = document.getElementById('canvas');
  if (canvas.getContext) {
    var ctx = canvas.getContext('2d');

    ctx.fillRect(25, 25, 100, 100);
    ctx.clearRect(45, 45, 60, 60);
    ctx.strokeRect(50, 50, 50, 50);
  }
}

## Drawing Paths
* Paths are a list of points, connected by segments of lines.
* There are 3 steps involved in making shapes with paths:
    1. create the path.
    2. use drawing commands to draw into the path.
    3. stroke or fill the path to render it.
* The functions we will use to achieve those steps include:
    - `beginPath()` // creates a new path. Once created, future drawing commands are directed into the path and used to // build the path
    - **Path methods**: Methods to set different paths for objects.
    - `closePath()` // adds a straight line to the path, going to the start of the current sub-path.
    - `stroke()` // draws the shape by stroking its outline.
    - `fill()` // draws a solid shape by filling the path's content area.
    - `moveTo(x, y)` // moves the pen to the coordinates specified by x and y.
    - `lineTo(x, y)` // draws a line from the current drawing position to the position specified by x and y.
    -  `arc(x, y, radius, startAngle, endAngle, counterclockwise)` // draws an arc which is centered 
        // (x, y) position   
    -  `arcTo(x1, y1, x2, y2, radius)` // draws an arc with the given control points and radius, connected to 
        // the previous point by a straight line.
    - to measure angles in the `arc` function we will use radians rather than degrees 
    - `radians = (Math.PI/180)*degrees` // converts degrees to radians

## Applying Styles and Colors

**Colors**

* `fillStyle = color` // sets the style used when filling shapes.
* `strokeStyle = color` // sets the style for shapes' outlines.

**Line Styles**

* `lineWidth = value` // sets the width of lines drawn in the future.
* `lineCap = type` // sets the appearance of the ends of lines.
* `lineJoin = type` // sets the appearance of the "corners" where lines meet.
* `miterLimit = value` // establishes a limit on the miter when two lines join at a sharp angle, to let you 
   // control how thick the junction becomes.
* `getLineDash()` // returns the current line dash pattern array containing an even number of non-negative numbers.
* `setLineDash(segments)` sets the current line dash pattern.
* `lineDashOffset = value` // specifies where to start a dash array on a line.

**Patterns**
* We can create patterns with the `createPattern()` method.
* `createPattern(image, type)` // creates and returns a new canvas pattern object. `image` is a `CanvasImageSource` 
// (an `HTMLImageElement`, another canvas, a `<video>` element) `type` is a string that indicates how to use the image.
* The type indicates how to use the image to create the pattern, and has to be one of the following string values:
* `repeat` // tiles the image in both vertical and horizontal directions.
* `repeat-x` // tiles the image horizontally but not vertically.
* `repeat-y` // tiles the image vertically but not horizontally.
* `no-repeat` // doesn't tile the image, used only once.
* Here is a `createPattern` example: <br />

function draw() {
  var ctx = document.getElementById('canvas').getContext('2d');

  // create new image object to use as pattern
  var img = new Image();
  img.src = 'canvas_createpattern.png';
  img.onload = function() {

    // create pattern
    var ptrn = ctx.createPattern(img, 'repeat');
    ctx.fillStyle = ptrn;
    ctx.fillRect(0, 0, 150, 150);

  }


**Drawing Text** 

* `fillText(text, x, y [, maxWidth])`// fills a given text at the given (x,y) position. Optionally with a
   // maximum width to draw.
* `strokeText(text, x, y [, maxWidth])` // strokes a given text at the given (x,y) position. Optionally with a 
   //maximum width to draw.

* Here is an example using `filltext` :
```
function draw() {
  var ctx = document.getElementById('canvas').getContext('2d');
  ctx.font = '48px serif';
  ctx.fillText('Hello world', 10, 50);
}
```

* Here's an example using `stroketext` :
```
function draw() {
  var ctx = document.getElementById('canvas').getContext('2d');
  ctx.font = '48px serif';
  ctx.strokeText('Hello world', 10, 50);
}
```
**Styling Text**
* Here are some properties we can use to customize text:
    - `font = value` // the current text style being used when drawing text. Default font is 10px sans-serif.
    - `textAlign = value` // text alignment setting. Possible values: start, end, left, right or center. 
    - `textBaseline = value` // baseline alignment setting. Possible values: top, hanging, middle, 
      // alphabetic ideographic, bottom. The default value is alphabetic.
    - `direction = value` // directionality. Possible values: ltr, rtl, inherit. The default value is inherit.
## Saving and Restoring State 

* `save()` // saves the entire state of the canvas.
* `restore()` // restores the most recently saved canvas state.
* A drawing state is made up of:
    - The transformations that have been applied (`translate`, `rotate` and `scale`)
    - The current values of the following attributes: `strokeStyle`, `fillStyle`, `globalAlpha`, `lineWidth`,  `lineCap`, `lineJoin`, `miterLimit`, `lineDashOffset`, `shadowOffsetX`, `shadowOffsetY`, `shadowBlur`, `shadowColor`, `globalCompositeOperation`, `font`, `textAlign`, `textBaseline`, `direction`, `imageSmoothingEnabled`.
    - The current clipping path

## Creating Charts With Chart.js

 * `Chart.js` is a JavaScript function that uses HTML5's `<canvas>` element we can use to create bar charts, bar charts, line charts, and more.

 **Drawing a Line Chart**

 1. For the first step we will need to add this to the body of our HTML page: <br />

 
 <canvas id="buyers" width="600" height="400"></canvas> 


 2. Then we need to write a script that will pull the context of our `<canvas>` element and put it in the foot of the body of our HTML page like so: 

```
<script>
    let buyers = document.getElementById('buyers').getContext('2d');
    new Chart(buyers).Line(buyerData);
</script>
```
3. Now we need to create our data inside the script tags, which ill be in the form of an object that contains labels for the base of our chart and datasets to describe the values on the chart. In this example, we need to add this immediately above the line that begins `var buyers=`: 

```
var buyerData = {
	labels : ["January","February","March","April","May","June"],
	datasets : [
		{
			fillColor : "rgba(172,194,132,0.4)",
			strokeColor : "#ACC26D",
			pointColor : "#fff",
			pointStrokeColor : "#9DB86D",
			data : [203,156,99,251,305,247]
		}
	]
}
```

**Drawing A Pie Chart**

1. Add the canvas element.
2. Get the context and to instantiate the chart.
3. Supply a color and value pair for each section.
4. After the data we will add our options, for example: 
```
var pieOptions = {
	segmentShowStroke : false, // remove the stroke from the segments
	animateScale : true // animate the scale of the pie so that it zooms out from nothing
}
```
**Drawing A Bar Chart**

1. Add the canvas element.
2. Retrieve the element and create the graph
3. Add in the data for the bar chart


