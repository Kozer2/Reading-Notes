DB Normalization

What is it? DataBase normalization is a way to reduce redundant data in your DB and to make it faster and more efficient. 
The more things a table covers the more convoluted it becomes and the harder it is to pull specific data out. 
In general, you want to have each table be for a specific thing. This helps reduce duplicate data in your tables.
To help normalize a Database we can follow the 3 form rule. 
Form 1:
- Has information stored in a table with each column containing values, it has no repeating columns of data.

Form 2:
- Table is the first normal form and all of its columns depend on the tables primary key

Form 3:
- This table is in the second normal form and all of its columns are not necessaily dependent on its primary key. 


For a form to be considered a 3rd form, it must also be able to be considered and first or second form. 
