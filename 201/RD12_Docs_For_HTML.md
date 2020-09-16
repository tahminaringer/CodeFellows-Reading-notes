# Reading 12 Docs For HTML

- Charts work better for dispaying data than tables
- **Chart.js** JS plugin that uses HTML5's canvas element to draw the graph onto the page.
  - makes using bar charts, line charts and pie charts more easy
**Setting up** download Chart.js
  - Copy the Chart.min.js out of the unzipped folder and into the directory you'll be working in
  - next create a new html page and improt the script
**Drawing A Line Chart** create a canvas element in our HTML in which Chart.js can draw our chart.`<canvas id="buyers" width="600" height="400"></canvas>`
  - add to the foot of your body element to retrieve the context of the canvas.
  `<script>`
    `var buyers = document.getElementById('buyers').getContext('2d');`
    `new Chart(buyers).Line(buyerData);`
`</script>`
  - inside the same scrpt tags we need to creat our data. 
**Drawing a pie chart** 
`<canvas id="countries" width="600" height="400"></canvas>`
- get the context and to instatiate the chart
- create the data
- add our options
**Drawing a Bar Chart**
`<canvas id="countries" width="600" height="400"></canvas>`
- add the canvas element
- retrieve the element and create the graph
- add in the bar chart's data

## Basic Usage Of Canvas

- `<canvas>` has two attributes width and height/ When no specifications standard is 300px wide and 150px high
- easy to define some fallback content
- element requires closing tag
  - Method- `getContext()` used to obtain the rendering context and its drawing functions takes one parameter.

## Drawing Shapes With Canvas

- **coordinate space** canvas grid
- **drawing paths** 
  1. create the path
  2. use drawing commands to draw the path
  3. once created you can strok or fill the path to render it
- `beginPaht()` creates a new path
- `Path methods` methods to set different paths for objects
- `closePath()` adds a straight line to the path, oing to the start of the current sub-path
- `stroke()` Draws the shap by stroking its outline
- `fill()` Draws a solid shape by filling the path's content area
`moveTo` similar to lifting a pen from one spot on a piece of paper and placing it on the next
  - x,y - moves the pen to the coordinates specified by `x` and `y`
`lineTo(x,y)` Draws a line from the current drawing position to the position specified by `x` and `y`
`arc(x, y, radius, startAngle, endAngle, anticlockwise)` draws an arc which is centered at (x, y) position with radius r starting at startAngle and ending and endAngle going in the given dirrection indicated by anticlockwise
`arcTo(x1, y1, x2, y2, radius)` Draws an arc with the given control points and radius, connected to the previous point by a straight line.
`quadraticCurveTo(cp1x, cp1y, x, y)` Draws a quadratic Bezier curve from the current pen position to the end point specified by x and y, using the control point specified by cp1x and cp1y.
`bezierCurveTo(cp1x, cp1y, cp2x, cp2y, x, y)` Draws a cubic Bezier curve from the current pen position to the end point specified by x and y using the controlpoints specified by (cp1x,cp1y) and (cp2x, cp2y)
`rect(x, y, width, height)` Draws a rectangle whose top-left corner is specified by (x, y) with the specified width and height.
`Path2D()` constructo returns a newly instantiated Path2D object, optionally with another path as an argument or optionally with a string consisting of SVG path data

## Applying Styles and Colors

- `fillStyle = color` sets the style used when filling shapes
- `strokStyle = color` sets the style for shapes outlines
- `globalAlpha = transparencyValue` applies the transparency value to all future shapes drawn on the canvas. 
- `lineWidth = value` sets the width of lines drawn in the vuture
- `lineCap = type` sets the appearance of the ends of lines
- `lineJoin = type` sets the appearance of the "corners" where lines meet
- `miterLimit = value` Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes
- `getLineDash()` Returns the current line dash pattern array containing an even number of non-negative numbers
- `letLineDash(segments)` sets the current line dash pattern
- `lineDashOffset = value` specifies where to start a dash array on a line.
- **Line Cap**
  - butt - The ends of lines are squared off at the endpints
  - round- the ends of lines are rounded 
  - square- the ends of the lines are squared off by adding a box with an equal width and half the height of the lines thickness
  - **LineJoin**
    - Round
    - bevel
    - miter
- Gradient-
  - `gradient.addColorStop(position, color)`creates a new color stop on the gradient object
- Patterns
  - repeat
  - reapeat-x
  - repeat-y
  - no-repeat
- **Shadows**
-`shadowOffsetx = float` indicates the horizontal distance the shadow should extend from the object
- `shadowblur = float` the size of the bluring effect
- `shadowColor = color` css color value indicationg the color of the shadow effect
**rules**
When using fill you can optionally provide a fill rule algorithm 
  - nonzero
  - evenodd

## Drawing Text

- `fillText(text, x, y [, maxWidth])` fills a given text at the given (x,y) position
`strokeText(text, x, y [, maxwidth])` strokes a given text at the given (x,y) position.
`font = value` the current text style being used when drawing text
`textAlign = value` text alignment setting
`textBaseline = value` baseline alignment setting
`direction = value` directionality
`measureText()` returns a TextMetrics object containing the width in px that the specified text will be when drawn in the current text style.

<form id='calculator'>
  <fieldset>
    <legend>Simple Calculator</legend>
    <p id="result">0</p>
    <label for="number1">
    Number
    </label>
    <input name="number1" id="number1" type="number" required>
    <button id="add-button">Add</button>
    <button id="sub-button">Subtract</button>
  </feildset>

```
var addButton = document.getElementById("add-button")
var subButton = document.getElementById("sub-button")
var numberImput = document.getElementById("number1")

function handleClick(event) {
var currentValue = parseInt(document.getElementById('result').textContent);
  event.preventDefault();
  var elementClicked = event.target;
  var elementClicked = event.target;
  var imputValue = parseInt(numberImput.value);
  var newValue = 0

  if (elementClicked.id === "add-button") {
    currentValueNum + imputValue;
  } else if (elementClicked.id === "sub-button") {
    newValue = currentValueNum - imputValue
  }
  currentValueEl.textContent = newValue
}

addButton.addEventListener('click', handleClick);
subButton.addEventListener('click', handleClick);

```
