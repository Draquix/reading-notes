## Reading Notes for JavaScript Chapters 3 and 5
Objects contain keys with values, which can hold anything a variable or array 
would, or even be a function- which makes it then called a method.  The 
properties of an object are accessed by dot notation in which the object is named
and a period follows with the key after. Object can be within objects, so one
call of a method could involve several periods and names.
The document object model is a hierarchy of the data structures that make up a
web page. The document has within the html which has within the body which has 
within the elements. Objects at the same level are siblings. Objects in another
are children of the parent.  The document can be manipulated by JavaScript by
directing focus to the node the element resides within and calling methods of the
document object

    var paragraph = document.getElementById("pick-this");

That code makes the paragraph variable get the node that contains the element 
whose tag has an id attribute set to 'pick-this'. The innerHTML method could be
called through dot notation, like paragraph.innerHTML = "Whatever you want the
paragraph to be displaying on the webpage itself."
Besides id, class, tagName, Css selector are other ways to access the webpage's 
content and alter it.  If a DOM query returns more than one element it becomes
a NodeList which is accessed the same as an array.
White space can affect getElementByTagName, especially the first and last child.
Accessing elements and nodes follows DOM structure and uses dot notation. The 
property, NodeValue contains the text content in that node. The property 
textContent or innerText can be used to change text.
Adding Elements: createElement(), createTextNode(), appendChild().

    var this = document.createElement('li');
    var text = document.createTextNode('content');
    this.appendChild(text);
    var position = document.getElementsByTagName('ul')[0];
    position.appendChild(this);

Above adds fills out content in an li and puts it in the ul on the page.

    var removeEl = document.getElementsByTagName('li')[3];
    var containerEl = removeEl.parentNode;
    containerEl.removeChild(removeEl);

Above removes the fourth li from the page.

getAttribute() will get an attribute such as class and the variable that gets it
can be manipulated.