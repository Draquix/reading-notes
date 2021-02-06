## Reading 01 | Code 301 | Responsive Web Design and Floats

### RWD
Within a year, mobile internet usage will surpass desktop usage.
Responsive Web Design is to make the internet/web content available to 
all users, regardless of device or screensize. 
Responsive is to react quickly and positively to change, and adaptive means to
be easily modified for a new purpose.
A flexible layout utilizes a grid that helps the website dynamically resize to
any width. They use % and em much more than px.
formula: target width / width of parent element = result of relative width
Media Queries are to specify styles for specific browsers.
the @media rule specifies a different stylesheet or block of CSS rules dependant on the result of a media query. -uses and, all, not, and only.
An initial-scale sets a default ration of design elements.  minimum-scale and maximum-scale define rules about how the layout changes in response to screen size
max-width:100% helps scale media within an element

### Floats
Float left  or right allows content to flow around the element.
An element with the 'clear' property will not move itself adjacent to the floated element, but will move down past.
A parent element containing all floats will have no height, and it affects backgrounds.
An empty div with clear after floated items/containers can prevent content from overlapping other elements.
Floats create alternate flows. Your code needs to account for normal, right, and left.


[SMACSS Handbook](smacss.com)
[An Article on Using Grids](https://css-tricks.com/dont-overthink-it-grids/)

