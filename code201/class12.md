# What I've Learned at the 12th lecture of 201 code

## Charts in JS

1. **Charts** are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool.

2. **Charts** are easier to look at and convey data quickly, but they’re not always easy to create.

3. *Drawing a line chart* :To draw a line chart, the first thing we need to do is create a canvas element in our HTML in which Chart.js can draw our chart.

4. *Usage of canvas* :At first sight a `<canvas>` looks like the `<img>` element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the `<canvas>` element has only two attributes, width and height.

5. The id attribute isn't specific to the `<canvas>` element but is one of the global HTML attributes which can be applied to any HTML element (like class for instance). It is always a good idea to supply an id because this makes it much easier to identify it in a script.

6. Required `</canvas>` tag As a consequence of the way fallback is provided, unlike the `<img>` element, the `<canvas>` element requires the closing tag (`</canvas>`). If this tag is not present, the rest of the document would be considered the fallback content and wouldn't be displayed.

7. **Drawing shapes with canvas**:

    - The grid
    - Drawing rectangles
    - Drawing paths

8. Colors: If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.

    - `fillStyle = color` :Sets the style used when filling shapes.
    - `strokeStyle = color`:Sets the style for shapes' outlines.

9.  > When you set the strokeStyle and/or fillStyle property, the new value becomes the default for all shapes being drawn  from then on. For every shape you want in a different color, you will need to reassign the fillStyle or strokeStyle property.

10. Color is a string representing a CSS `<color>`, a gradient object, or a pattern object.

11. The valid strings you can enter should, according to the specification, be CSS `<color>` values. Each of the following examples describe the same color.

    - ctx.fillStyle = 'orange';
    - ctx.fillStyle = '#FFA500';
    - ctx.fillStyle = 'rgb(255, 165, 0)';
    - ctx.fillStyle = 'rgba(255, 165, 0, 1)';

12. **Drawing text** The canvas rendering context provides two methods to render text:

    - fillText(text, x, y [, maxWidth]): Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.

    - strokeText(text, x, y [, maxWidth]): Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

13. A fillText example:

    >function draw() {  
    var ctx = document.getElementById('canvas').getContext('2d');  
    ctx.font = '48px serif';  
    ctx.fillText('Hello world', 10, 50);  
     }

14. A strokeText example: 

    >function draw() {    
    var ctx = document.getElementById('canvas').getContext('2d');    
    ctx.font = '48px serif';    
    ctx.strokeText('Hello world', 10, 50);  
   }

15. **Styling text** :  There are some more properties which let you adjust the way the text gets displayed on the canvas:

    - font = value
    - textAlign = value
    - textBaseline = value
    - direction = value


### RESOURSES

 - [article](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/) 
 - [Chart.js](https://www.chartjs.org/docs/latest/)
 - [Basic usage](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage)
 - [Drawing shapes with canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)
 - [Applying styles and colors](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors)
 - [Drawing text](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text)