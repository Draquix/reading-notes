## Reading Notes 09 | Code 301 | Functional Programming
*readings from*: [Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)
and, [Refactoring JavaScript for Performance](https://dev.to/healeycodes/refactoring-javascript-for-performance-and-readability-with-examples-1hec)

**the first article asked me to pay for membership since I'd read all the free stories I'm allowed?**

When iterating through an array too often, it can slow down the program- especially if it's a big array.
The datatype can be converted using a hash function, like making a const of the array using .map.

When several functions are doing similar jobs, thus creating redundant code, its best to combine them into a single function the takes a larger set of data or more parameters to do multiple tasks with the same function.
If there's a large function doing several things, and you have what you need, you can use an if statement to check for a condition to have been met and if so, return;.  
Variable names should reflect what they're doing so the code can be read like sentances, even if it means adding lines in which const something = whatItRefersTo[x];

[Back to Table of Contents](../README.md)