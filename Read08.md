## Conditions and Loops

#### Condition Statements
Often a program must evaluate data and make decisions based on
whether a statement is true or false, or dependant on what a 
numerical value is. The 'If' statement makes use of this. Other
times evaluations are made are in loops in which the program 
will keep executing a block of code as long as a certain 
condition is or isn't met.
###### Table of Conditional Operators
==  : is equal to  ,  === : strict equal to (used in if statements checking a boolean value)
!=  : is not equal to ,  !=== : strict not equal to
*note on equal to and not equal to, it will compare an integer and a string with a number in it and evaluate as true 
ie: 42 == '42' is true, whereas 42 === '42' is false.
> : is greater than  ,  < : is less than
>= : is greater than or equal to  ,  <= is less than or equal to
###### Table of Logical Operators
&& : and   ,   || : or  ,  ! : not
ie: while (x >= 3 && y < 5 || lifeMeaning === 42) {code to be run}
That statement would read as while x is greater than or equal 
to 3 and y is less than five or lifeMeaning is 42, keep 
executing the block of code in the curly brackets until one or 
more of those comparison statements is no longer true. For 
instance if the block of code changed the variable y to 6, it 
would stop executing that block because y is no longer less 
than five. Or nothing could happen numerically to x or y to no 
longer satisfy the conditions of the while loop but the 
lifeMeaning variable became anything other than the strict 
numerical value of 42, that could also stop the while loop. 

[Back to Main Page](https://draquix.github.io/reading-notes-javascript-102/)
