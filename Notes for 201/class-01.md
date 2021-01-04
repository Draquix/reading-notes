## Initial Reading Assignment from Ducket books
#### Chapters 1, 8, 17, 18 in HTML book and Introduction and Chapter 1 in JS book

### HTML Chapter 1
HTML is used to give structure to the content of the page.  The content within tags is called elements. The tags consist of a keyword with 
attributes that together determine how the content is displayed in terms of visual appearance and location. An attribute is made up of its name 
followed by an equals sign and a value within quotemarks. A web browser reads the HTML page and displays its content. An HTML file, in its raw 
form, is mostly unformatted text. The tags and their attributes are brackete within greater than and less than signs. A tag often has an 
opening tag followed by it's content and an ending tag that is the tag name preceeded by a forward slash. When the web browser reads the HTML 
document, it follows the prescribed guidelines dictated by the HTML tags to format and structure its elements and displays that content with 
the ommission of the HTML tags themselves. For example the element of a paragraph, has the opening tag, <p> and the ending tag </p>. Between 
the two tags is the text of the paragraph. The web browser displays the text as a paragraph without showing the <p> tags.

### HTML Chapter 8
There have been several versions of HTML since its conception. We currently use HTML which is denoted by the <!DOCTYPE html> tag as the first 
thing within the document. Comments, which are statements that exist only within the HTML code, meant to communicate with other programmers who 
may view the source, are bracketed within <!--   comment goes here --> tags. An element can contain an id attribute, which can be used by CSS 
or JavaScript to targeted and modified specifically. One id can apply only to one element. A class attribute is much like an id, but may be 
common to multiple elements within a page. For instance if you have ten <p> tags on a page, one of them may be singled out by a CSS rule for 
styling or a JavaScript program to have its content altered by having an id, whereas three or five or all of those <p> tags can share a class 
to identify them. Some elements are used for grouping other elements within them together like <div>.
Elements are either 'block' or 'in line'. Block elements are considered as if within a block, they have a border and a margin and unless 
certain CSS styling rules are applied, they appear above and below each other. In line elements can be side by side, as if words next to each 
other within a sentance. One type of block element is an iframe, which functions as a smaller window of content within the larger window of the 
page.

### HTML Chapter 17
In HTML5 some new grouping elements have been implemented to replace the previous over-use of the <div> tag. There are now specific elements 
for a header or footer or nav bar to reflect commonly used themes standard to how the WWW usually presents its pages. Sometimes, older browsers 
do not treat properly newer block elements as they're meant to be displayed so certain CSS rules can be applied to help them understand. In 
many ways, the newer semantic tags for grouping elements perform the same as the old method of using <div> for every grouping, but the newer 
method helps organize the code in a way that helps developers and readers better understand the intent of the usage of the grouping.

### HTML Chapter 18
When creating a website, you should think about your audience and pitch the content to them as they want to see it and help them focus on the 
information they're seeking. Sometimes people will create lists of fictional people to assist in narrowing down their audience. A site map is a 
visual representation of the pages in a branching structure like a tree, with the main page being the trunk. A wireframe is a design tool in 
which the page is drawn as an artistic rendering to plan how it will appear before tags and elements and content are all begun being structured 
by the HTML code. The artistic nature of the page could and should be usec to direct someone's attention in their aid and in the aid of the 
owner of the site. Likened information should be grouped together, and colors should be both attractive as well as contrasting to make it 
readable. Common themes like a navigation bar should help users achieve their purpose in getting around the site.

### JS Chapter 1
A script is a series of instructions. JavaScript is generally used to make a page interactive, by altering or producing content based on a user's actions. A script achieves an intended goal step by step. A flowchart is a visual representation of the steps involved in the code attaining its goal and is used in the planning stages. Computers store the world as data. Information about specific concepts is grouped together as objects and each piece of data, like color of something or its size, is a property. A method is an instruction that carries out a task. An object is a collection of properties and methods. A web page is an object, and its content are properties, and the most basic interactive element, the hypertext link, is a method of connecting a page to another and transporting the user there. A JavaScript program can be embedded between a <script> and a </script> tag directly in the HTML file. A script can also be contained in an external source file and linked with a tag that has the path to the file. The latter is considered better practice. A page is loaded from top to bottom, and a script is executed when encountered, so when using a larger script it's best to be placed at the bottom of the page so all the visual HTML elements load and display while the computer's memory is processing the script.