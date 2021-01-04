## Reading Notes 05
#### Introduction to CSS

There are two categories of HTML elements: block and inline. 
Inline elements do not start a new line and do not have a box 
around them. Block elements are treated as if there is a box 
around the element. With CSS you can change the box's position,
size, add borders, and color scheme within.
A CSS rule has two parts: the selector and the declaration. A
selector is a tag name, or if and ID or Class attribute have
been set within the HTML that can be used as the selector. The
selector tells **what** the rule is applying to. The declaration 
contains properties and values. The property may be *height*, or
*border*, or *position*.
Example of a CSS rule:
    main {
        width:300px;
        color:red;
        background-color: black;
    }
In this example, everything within the <main> tag will have a 
black background with red text and the block defining the size
and layout of the main element will be only 300 pixels wide. An 
average screen length is 6-700 pixels, so our element would be
quite scrunched up, but we're just trying to explain a general 
rule. Part of the syntax is that the selector is followed by 
curly braces ( {} ), within those braces are the declarations.
The property is written to the left followed by a colon, and then
the value of that property is typed followed by a semicolon.
By using a <link> tag, an external file.css file can store all
the CSS, or you can do it right in the HTML with a <style>
</style> set of tags- however this is not recommended practice.
There are several types of selectors. If you wanted to select a
<p> tag, but only the <p> tags inside an <article> your selector 
would be article p {}... if an id attribute is set in the HTML 
like <p id="this-one"> or class attribute like, 
<p class="that-one"> the selector could be very specific to that 
one element by .this-one {} or #that-one {} respectively.
CSS will apply first to the broadest scope set, like body {} and 
then if there's a <h2> within that body that gets called by its
selector and has a different rule that narrower definition will
overwrite the rules set by the broader selector's rule.

In CSS we often change the color of text or a background or a 
border around a box. Some specific color names: red, blue, 
lightgreen etc can be used as the value of a color property. To
go beyond the basic predefined palet we can also use RGB 
followed by 3 numbers between 0 and 255. It stands for red,
green, blue and works much like mixing paint where the higher
the numerical value the more of that color paint we're mixing in.
As black is the absence of light(thus color), the RGB for black 
is 3 zeros. Similarly since white light is the entire spectrum
combined, its RGB is 255,255,255. Aside from direct names or RGB,
we can define colors by a hex code which is delineated by a 
number sign and then six alphanumericals pertaining to a 
hexidecimally referenced color.
When choosing a color scheme one should pay attention to the 
contrast of the background and foreground. Green text on a
blue background would be quite illegible. Personally I love red
or green on black as a throwback to old computers that 
preexisted the GUI age when macintosh came out, followed by 
windows.

[Back to Main Page](https://draquix.github.io/reading-notes-javascript-102/)
