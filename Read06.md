## Reading Notes 06

### About JavaScript 

Where HTML provides structured content, and CSS gives the page style and an 
attractive look, JavaScript makes a page interactive. JavaScript is a script, not 
a language that gets precompiled into an application in a .exe form.  Being a
script, it gets executed by the browser on the client side. It can communicate
with back end server programs as well, but it is running on the client's browser.

JavaScript is what makes a page do something. It is Object Oriented in a way that
is similar to C++ or Java. An object is a collection of keys and values. It runs 
functions much like other programming languages which is a grouped set of commands
that are executed together, and can return a result to the rest of the program.

JavaScript is added by the <script></script> tag. Commands can be nested between 
the tags, but it is better to use an attribute src='filename.js' in the script 
tag to link to external .js files. Below is a sample function:

<p id="place-holder"> ... </p>
<script>
function replaceElipsesWithHello() {
    var message = "Hello World";
    document.getElementById('place-holder').innerHTML = message;
}
replaceElipsesWithHello();
</script>

Function tells the interpreter we're making a new function. var initializes a 
variable, and in this instance it's called message. The variable is assigned
a value that is a text string, as denoted by the quotes. Commands are proceeded by
a semicolon. document.getElementById looks for the html element that was given the
id that it's given in single quotes and innerHTML and sets the HTML inside the tag
that was looked for. In this case it's being set to the variable message. The 
function's statements are enclosed in curly braces. After the curly brace closing
the function we actually call the function with it's name and parenthesis.

[Back to Main Page](https://draquix.github.io/reading-notes-javascript-102/)
