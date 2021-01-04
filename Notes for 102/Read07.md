## Notes on Scripts, Expressions, and Functions
#### Pages 1-24, 74-9, 88-94

Javascript is integrated with HTML and CSS in a way that it can
access content, and modify it, or react to events like user 
input or perhaps the time of day.

### Scripts
A script is a list of instructions in the JavaScript language. 
For the most part it is executed in the order it is written from
the top of the page to the bottom. An exception to this is a 
function may be written near the beginning of the script and 
then called further into the script so that those grouped 
statements were executed- but after that the execution would 
return to the place from which the function was called.
When planning to write a script, the programmer should first 
define the goal of the program. Then they should list the steps
needed to reach that goal- and those steps should be very simple
and literal as the computer will do exactly what it is told to 
do without any intuitive alteration of the instructions as a 
human would make.

### Expressions
Espressions are comprised of either assigning a value to a 
variable, or evaluating two values to produce a single result.
For instance the expression var x = 2; would initialize the 
variable x and assign it the property value of the number two.
var sum = x + 10; would calculate what x (in this case it's 2) 
plus 10 evaluates into which is 12, and then it assigns the sum
variable that value of 12.
Operators are ways to manipulate data and include the plus or 
minus sign, an asterix and foward slash for multiplication and
divide respectively, or even an equals sign which we call the
'asignment operator' as it will asign a value to a variable. 
Some operatiors can be used on strings too, it's not just about
numbers! For example var msg = "Hello " + "World!" would let the
variable message contain a single string: "Hello World!".

### Functions
A function is one or more statements grouped together, generally
because they collectively fulfill some objective of the code.
The keyword 'function' followed by the name of the function and 
then two parentheses within which parameters (more on those in 
a second) may or may not be set and the the curly brackets 
within which the statements are grouped is the basic structure 
of a function.
function example(numOne,numTwo) {
    var sum = numOne + numTwo;
    document.write("The sum of the numbers is: "+sum);
    var product = numOne * numTwo;
    document.write("The product of the two numbers is: "+product);
}
numOne and numTwo are parameters. They work much like variables 
but their values can be passed in the statement calling the function. ie: example(3,4); would execute the function which 
would in turn carry out it's instructions to add those numbers
and assign them to sum, which is written to the document object 
as 7, and then it would multiply them and assign that to product
and then the last statement would write 12 to the document. The 
curly brackets encapsulate the statements of the function and 
only get executed if/when the functions gets called. If that 
function was in a script, but nowhere in the script was there a
statement: example(x,y); it would never be used.
A further rule to note about functions is that they can not be
called earlier in a script than they are declared. In my 
personal practice I first declare all my global variables at the
very beginning of the script, and then I write out all my 
functions so they are registered by the browser, and after that 
I put the statements to be run regardless of input or 
circumstance in the order they should be carried out, and those
statements are what typically call upon the functions I've 
defined above the active portion of the script.

[Back to Main Page](https://draquix.github.io/reading-notes/)
