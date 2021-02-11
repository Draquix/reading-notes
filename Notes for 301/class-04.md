## Reading Notes 4 | Code 301 | Responsive Web Design and Regular Expressions

Inside parenthases and square brackets a range of letters can be specified. ie: ([a-f]) to be matched.
[^lmnop] the carrot symbol indicateds letters to exclude from the search.
[abc] single characters can be specified
[abc\s]would match the characters without a line break , \w matches to a word, \W matches not a word
\d matches a digit, \s is whitespace \S is not whitespace
[\p{Ll}] the \p specifies the character p and in curly brackets a unicode type, Ll would be all lowercase

From another reference, ^The looks for strings starting with 'The'  and end$ finds a string ending with 'end'
abc* matches a string 'ab' with zero or more 'c'
abc+ matches a string 'ab' with one or more 'c'
abc{2} matches a string with ab followed by 2 c's
abc{2,} matches a string with ab followed by 2 or more c's
{2,5} looks for there to be from 2 to 5 of the last character

[abc] looks for a string with a, b, OR c


#### Grids:
display can be set to 'grid' or 'inline-grid' for a parent container element
grid-template-(columns/rows): track-size is a length, percentage, or fraction -fr- that defines the size of the grind,  or a line name can be chosen to refer to by children

children elements can set values to the properties of 'grid-column-start', 'grid-column-end','grid-row-start', and 'grid-row-end'
 the values children can be set to are line, span < name / number >, and auto 

In article [Common Responsive Layout with CSS grid](https://github.com/Draquix/data-structures-and-algorithms/pull/3) by Jo Franchetti,
A responsive page design using grid showed a larger header image at the top of the page with smaller images that are two-across on smaller screens and as they all expand, there gets to be 3 or 4 of the smaller images at specific breakpoints.
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
The author states that "the repeat() function takes two arguments, the first will define the number of column tracks and the second, what width the tracks should be."
By using auto-fill it will make the grid with as many tracks as will fit the container, and minmax means they are a minimum of 250px wide.  the max of 1fr is that if there is space for 2 250px rows (2/2) there would become 2 rows. so at 750px there are now 3 rows that scale with the page until 1000px at which time there are four.
the author uses   object-fit:cover;  to make sure cropping doesnt occur.

Several other layouts are given at this site, and they are MIT!!!:) license, so us junior developers are free to borrow their code and experiment or expand upon it with our own.

[Back to Table of Contents](../README.md)
