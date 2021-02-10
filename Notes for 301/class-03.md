## Reading 03 | Code 301 | Flexbox and Templating

### Required Reading Articles Linked Below:
* [Templating with Mustache](https://1sherlynn.medium.com/javascript-templating-language-and-engine-mustache-js-with-node-and-express-f4c2530e73b2)
* [Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
* [FLexbox Froggy](https://flexboxfroggy.com/)

#### Templating and Mustache
*Some paraphrasing done from the above-linked article by Sherlynn Tan*
Templating renders content to the page using a JSON source file. 
A template is standard HTML, but extra tags are put in that are used as placeholders for variables or trigger codeblocks to be run within the program.
Mustache is a way to put extra tags in templates that the program replaces with data or removes. It is an external library: mustache.js.
It works by using double curly braces to mark a point of insertion.
With the library linked, the syntax is to use
   
    res.render('nameOfHTMLfile', {"key": "valuePair"})
    //or declare a var/const and assign it JSON data
    const dataBit = {"hornedThing": "unicorn"};
    res.render('index', dataBit)

in the HTML: 
    
    <h2>This thing is named {{hornedThing}}</h2>

and the result is the header2 will say 'This thing is named unicorn'.

#### Flexbox
**Set display**:*flex*; on the parent element to enable flex content for all direct children.
Content is layed out in a direction that can be specified by setting **flex-direction** to either *row*, *row-reverse*, *column*, or *column-reverse*.
**flex-wrap** is set to determine if it may use another line or not through, *nowrap/wrap/wrap-reverse*
**justify-content** can be left, right, or center with *flex-start/flex-end/center* or set to *space-between, space-around,* or *space-evenly*.
**align-items** affects vertical actions, *flex-start* or *flex-end* cause either the top or bottom margins to align. *center* uses the median height, *stretch* adjusts height to fit the parent, and *baseline* uses an inner textual reference to align.
**align-content** uses same settings as align-items
##### Children Properties:
The children of a flex box have a property: **order** which is a numerical value.
**flex-grow** is by default 1, and has no unit, it's a proportional measurement by which they are resized to fit
**flex-shrink** is the opposite of flex-grow and may not use negative values.
**flex-basis** uses standard units to determine a default size before the rest of the space is distributed to other children
**align-self** uses the align-items attributes, but specific to the child.

#### Note About Flexbox Froggy
It's pretty intuitive and levels 1-23 took 15 seconds to a minute... but I was on level 24 for about half an hour before I came up with:
    flex-direction:column-reverse;
    flex-wrap:wrap-reverse;
    justify-content:center;
    align-content:space-between;
But it was kind of fun.

[Back to Table of Contents](../README.md)
