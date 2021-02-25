## Reading Notes 14a | Code 301 | Database Normalization
[Source Article](https://www.essentialsql.com/get-ready-to-learn-sql-database-normalization-explained-in-simple-english/)

Database normalization is to organize the contents into tables and columns.
A table should be specific to a topic.
Limiting the scope of a table helps avoid redundant data.
Database normalization also simplifies queries.
Duplicate information increases storage space, slows down performance, and makes it more difficult to maintain changes.

An insert anomaly is when you need all the information in the row to look it up.
An update anomaly is when multiple rows need changed and aren't all updated.
A delete anomaly is when removal of data removes other data as well.

First Normal Form- The information is stored in a table with no repeating groups of columns.
A table of the Second Normal Form is organized based of its primary key.
The Third Normal Form is for a table to be organized according to the Second but not dependent on the primary key.
