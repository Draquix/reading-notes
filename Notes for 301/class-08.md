## Reading Notes 08 | Code 301 | SQL
source reading: [Sql Bolt Docs](https://sqlbolt.com/)

SQL stands for Structured Query Language.
It is formatted as a table of related entries of fixed properties and attributes per entry.
#### basic query
Using SELECT column, another column   FROM myTable   --> will return the properties of those columns for all entries in the table.
An asterix will select all.
adding conditions can be done using WHERE condition AND/OR condition AND/OR another condition
SELECT DISTINCT col, col2   will remove duplicate columms
ORDER BY col ASC/DESC lists the returned entries in ascending order by that column
LIMIT specifies the number of entries to return
OFFSET specifies the number of the row to begin counting from
#### operators in queries
operators =, !=. <, <=, >, >=   can be between parameter/variable names and numbers
BETWEEN ... AND  specifies a range of 'col_name' entries
NOT BETWEEN ... AND specifies outside a range
IN ()  finds numbers in a list ie: (1,2,5,9)
NOT IN () excludes the items in the list
LIKE  will compare two strings with case insensitivity
NOT LIKE will compare two strings and return those without the strings
% can be used to match a sequence of zero or more characters with LIKE or NOT LIKE :  col_name LIKE "%AT%" matches "AT", "ATTIC", "CAT", or "BATS".
_ can be used to match any single character in a string : col_name LIKE "DA_" matches "DAN" but not "DA".

[Back to Table of Contents](../README.md)