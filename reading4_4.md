# Data Modeling

## nosql vs sql

1. What type of database is the best fit for the complex query intensive environment?

- SQL databases

2. What type of database is the best fit for hierarchical data storage?

- NoSQL databases

3. Describe the differences in scalability between a SQl and NoSQL database as though you were speaking to a non-technical friend.

- NoSQL is better if you would rather add more servers to handle more data while SQL is better if you increase the storage and speed on a single server

## sql modeling techniques

1. Among data tables, what is a one-to-many relationship and how do we “relate” them?

- We connect lines between tables to show relationships. In some cases an entry in one table can be related to more than one entry in another.

2. Prior to designing your relational database, it might be useful to ___a___ of the database tables and their relationships.

- create a diagram

3. Explain the difference between a primary and foreign key.
-The Primary Keys. Remember the primary keys uniquely identify each row in a table. A table typically has one primary key, but can have more.

- Foreign Key – This is a column or set of columns which match a primary key in another table.

## sql vs nosql

1. How do we treat keywords and parameters differently in SQL syntax?

- They are very specific in there intent especially when creating new tables and data

2. Define normalization within the context of schemas and data.

- The goal of normalized schemas is to avoid the storage of duplicate data so that stored data can't become inconsistent.

3. Explain the difference between one-to-one, one-to-many, and many-to-many relationships to a non-technical recruiter.

- One-to-One relationship, one record of the first table will be linked to zero or one record of another table.
- One-to-Many is the most commonly used relationship among tables. A single record from one table can be linked to zero or more rows in another table.
- Many-to-Many relationship lets you relate each row in one table to many rows in another table and vice versa.
