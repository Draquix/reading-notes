## Notes for Class 12 - Docs for Chart.js and asst Articles on the Canvas API

This plugin draws charts onto a canvas.  First the .js needs to be linked to a
script tag either by download or external link. Next we need a canvas tag on the
html page.  There is a slightly different way to call each type of chart.
In all a var is declared that uses getElementById to grab the id of the canvas
and a new Chart object is declared of the type desired.  The charts take arrays
of numbers or objects that specify datavalues as well as colors to be used in
representing that data visually.

The canvas element creates a box of specified width and height. Fallback content
to be displayed if the canvas isn't supported can be inserted between the open 
and closing tags.  A method, getContext() takes the parameter of '2d'. when a
var is set to this method it can be used to call drawing methods:

    var canvas = document.getElementById('canvas');
    var ctx = canvas.getContext('2d');

    ctx.fillStyle = 'rgb(200, 0, 0)';
    ctx.fillRect(10,10,50,50);

this will choose the color red and draw a rectangle using the x,y,width,height 
properties in pixels.
Canvas can only draw rectangles or paths, which are series of connected lines.
In paths:
    beginPath() creates a new path
    moveTo(x,y) sets begin point by moving the pen, so to speak
    lineTo(x,y) draws a line from previous point to the new one
    closePath() adds a straigth line to the path
    stroke() draws an outline of a shape
    fill() draws with a solid color

Colors can be specified for the fill using standard rgb, rgba, hex methods in
CSS.  
Line styles can be set to have different widths, can be dashed with various 
patterns.
Text can be drawn with fillText(text,x,y). by using ctx.font = 'css value' the
font can be customized.

[Back to Table of Contents](../README.md)

    