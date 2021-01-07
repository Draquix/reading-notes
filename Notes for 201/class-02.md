## Reading Notes for Duckett HTML Chapters 2 and 10

Text can be manipulated in many ways with HTML. Tags such as bold, italic, strong, and emphasis change the appearance of the text.
Tags can be used to make super or sub script. Abbreviations and acronyms can be set to display the full text they represent upon mouse hovering over.
There are tags that handle quotes and citations as well. Although HTML ignores white space, it can style or structure text in many of the ways
a word processor can as well as some extra features when the mouse hovers over certain tags.

In CSS every element has a box around it with an allotted inside space called padding, and a border (which is often invisible), and a margin that 
dictates how far away the box of another element has to be from it. A stylesheet is a list of what are calle rules. The rules format
the size of the boxes, and the appearance.  In the stylesheet one targets a specific element by name as the selector, and then within { } brackets
there are properties and values. A property may be color and after a colon there is typed purple. The text of the element that was
selected would appear purple. Usually we want to use a link tag within the head tags of the document that names the separate file that can sometimes
be multiple pages of CSS rules. But if we're just changing one little thing, or other special circumstances a style tag can be used and within its
opening and closing may be selectors with thier properties and values.  In HTML we often encounter elements within elements. The order in which the 
stylesheet writes rules matters in that the last rule encountered is the one that takes precedence, as is the most specifically targeted element's
selector.

## Reading Notes from the JS book, Chapters 2 and 4

JavaScript is, at it's most basic level, made up of statements that change or do one thing within the program and they end with a semicolon.
To leave notes for other developers who may look at your code, we can use two forward slashes for one line, or a forward slash followed by
an asterix for multiple lines, and none of the commented code will be run. We use variables to store bits of information. They need to be declared
with the var keyword and to be of use they need to be assigned a value. The value of a variable can be of varying data types, like a number or a 
string of text or a boolean value like true. Another way to store data is an array, which is like a list of different values. The first value is
listed at 0, not one as many humans would think. To access an array we use its name and the index number of the desired value within brackets.
In JavaScript we manipulate numbers, and the language allows for most mathematical operations to be carried out using operators like the plus 
sign or an asterix to multiply or slash to divide.

JavaScript follows the script in order from top to bottom. It cannot do the next instruction until it finishes with what it's doing. 
Since functions call upon instructions elsewhere in the code, there is a concept of a stack. When a function calls upon a new set of
instructions it takes precedence, and when finished the next instruction after the function was called is the top of the stack.
Variables have a limited scope, when declared within an object they don't exist outside of that object. When we make errors the JavaScript
interpreter stops executing the code and gives a message that identifies the factor that is wrong. Debugging is done by trying to understand
what generated the error message, and can be aided by a console in the web browser that can manipulate the code or have status messages
logged into it. 

[Back to Main Page](https://draquix.github.io/reading-notes/)

