# Chart.js

#### Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.

#### A great way to get started with charts is with Chart.js, a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy.

![Image](https://cdn.mos.cms.futurecdn.net/S5bicwPe8vbP9nt3iwAwwi.jpg)

## Drawing a line chart
- To draw a line chart, the first thing we need to do is create a canvas element in our HTML in which Chart.js can draw our chart. So add this to the body of our HTML page:

**(canvas id="buyers" width="600" height="400"></canvas)**   

- Next, we need to write a script that will retrieve the context of the canvas, so add this to the foot of your body element:

**(script>
    var buyers = document.getElementById('buyers').getContext('2d');
    new Chart(buyers).Line(buyerData);
</script)**

----

## The canvas element

*At first sight a **canvas** looks like the **img** element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the canvas element has only two attributes, **width** and **height**. These are both optional and can also be set using **DOM** properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn't respect the ratio of the initial canvas, it will appear distorted.*

### The rendering context
- The canvas element creates a fixed-size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown. 

- The canvas is initially blank. To display something, a script first needs to access the rendering context and draw on it. The canvas element has a method called getContext(), used to obtain the rendering context and its drawing functions. getContext() takes one parameter, the type of context. For 2D graphics,  you specify **"2d"** to get a **CanvasRenderingContext2D.**

----

## Drawing shapes with canvas

### The grid

- Our HTML skeleton had a canvas element 150 pixels wide and 150 pixels high.
- Normally 1 unit in the grid corresponds to 1 pixel on the canvas. The origin of this grid is positioned in the top left corner at coordinate (0,0)
- All elements are placed relative to this origin. So the position of the top left corner of the blue square becomes x pixels from the left and y pixels from the top, at coordinate (x,y). 

### Drawing rectangles
- canvas only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths. Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes.

- There are three functions that draw rectangles on the canvas:

1-**fillRect**(x, y, width, height)  
Draws a filled rectangle.  
2-**strokeRect**(x, y, width, height)  
Draws a rectangular outline.  
3-**clearRect**(x, y, width, height)  
Clears the specified rectangular area, making it fully transparent.  

- Each of these three functions takes the same parameters. x and y specify the position on the canvas (relative to the origin) of the top-left corner of the rectangle. width and height provide the rectangle's size.

![Image](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes/canvas_default_grid.png)

### Drawing paths
 - A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. A path, or even a subpath, can be closed. To make shapes using paths, we take some extra steps:

1- First, you create the path.  
2- Then you use drawing commands to draw into the path.  
3- Once the path has been created, you can stroke or fill the path to render it.  
Here are the functions used to perform these steps:

**beginPath()**  
Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.  
**Path methods**  
Methods to set different paths for objects.  
**closePath()**   
Adds a straight line to the path, going to the start of the current sub-path.  
**stroke()**  
Draws the shape by stroking its outline.  
**fill()**  
Draws a solid shape by filling the path's content area.

---

## Applying styles and colors

 - we will use styles and colors to make our drawings a little more attractive. 

- If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.

**fillStyle = color**  
Sets the style used when filling shapes.  
**strokeStyle = color**  
Sets the style for shapes' outlines.  

- color is a string representing a CSS <color>, a gradient object, or a pattern object

### Colors
- When supplying colors to Chart options, you can use a number of formats. You can specify the color as a string in hexadecimal, RGB, or HSL notations. If a color is needed, but not specified, Chart.js will use the global default color. There are 3 color options, stored at Chart.defaults, to set:

Name | Type | Default | Description
----|-----
backgroundColor |Color| rgba(0, 0, 0, 0.1) | Background color
borderColor |Color| rgba(0, 0, 0, 0.1) | Border color
color |Color| #666 | Background color

- You can also pass a CanvasGradient object. You will need to create this before passing to the chart, but using it you can achieve some interesting effects.

![Image](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors/canvas-grid.png
)

### Patterns and Gradients
- An alternative option is to pass a CanvasPattern or CanvasGradient object instead of a string colour.

- For example, if you wanted to fill a dataset with a pattern from an image you could do the following.

    var img = new Image();
    img.src = 'https://example.com/my_image.png';
    img.onload = function() {
    var ctx = document.getElementById('canvas').getContext('2d');
    var fillPattern = ctx.createPattern(img, 'repeat');

    var chart = new Chart(ctx, {
        data: {
            labels: ['Item 1', 'Item 2', 'Item 3'],
            datasets: [{
                data: [10, 20, 30],
                backgroundColor: fillPattern
            }]
        }
    });
};
---

## Drawing text
- The canvas rendering context provides two methods to render text:

**fillText**(text, x, y [, maxWidth])    
Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.  
**strokeText**(text, x, y [, maxWidth])  
Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

## Styling text

**font = value**  
The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.  
**textAlign = value**  
Text alignment setting. Possible values: start, end, left, right or center. The default value is start.  
**textBaseline = value**  
Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.  
**direction = value**  
Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.