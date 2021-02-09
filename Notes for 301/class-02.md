# Reading 02 | Code 301 | JQuery, Events, and the DOM

### Duckett JS/JQuery book pgs 293-301, 306-331, and 354-357

The function JQuery() lets you find elements easier, handle events in more simple way, and do animations
The $ is shorthand for it: $(#ElementId , .class) would select an element with the id Element Id, as well as any class that is named class.
For the most part, the selectors for JQuery are like the ones for CSS
$().addClass() will add a class to the elements selected
The library needs to be linked with a script tag before any other JS script is linked that utilizes it.
JQuery's library has built in feature detection so it works for all browsers

For JQuery selections of multiple items, a method used to gain info will only return about the first element
But if JQ method is used to update/change attributes of a selector returning multiple elements, it will affect all of them.
Storing references in a variable requires less memory, and those variables usually start with $ to denote they're JQuery references.
*implicit iteration* is JQ's ability to update multiple objects with a single selection
*chaining* is to use dot notation that calls multiple methods upon the same selection, as below:
    $(p.class).hide().delay().fadeIn(##mms);
methods that retrieve info cannot be chained.
To wait to run the JQ script after everything is loaded, a function is used as below:
    $(document).ready(function() {
        //write the script here
    })

### Methods:
.html() will return all the HTML, as in the tag and then the content between and the ending tag.
.text() will return just the text between the tags
.append() adds content to the end of the element.
.replaceWith() replaces every element in a set and returns the replaced elements
.remove() removes all elements in set
.before()/.after()  inserts content before/after selected elements
.prepend() inserts content inside element before closing tag
.attr() get or set a specified attribute
.removeAttr()  removes attribute
.addClass/.removeClass  adds or removes a class from element

#### Create Element in JQuery
    $newThing = $('<p id="new-paragraph"> Bunch of text for paragraph</p>' );

.each( function() {//block of code to perform}) runs a block on each element in a group
.on('event',function() {//code to run as event handler})

Event handling functions recieve an event object that has methods and properties accessed through dot notation
Effects and transitions are easily accessed in JQ
.animate({ //styles you want to chang}speed,easing,complete)
The DOM can be accessed by .parents() or .siblings()

[Back to Table of Contents](../README.md)