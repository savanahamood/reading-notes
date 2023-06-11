# SQL vs NoSQL
1. What type of database is the best fit for the complex query intensive environment?
SQL DataBase.

2. What type of database is the best fit for hierarchical data storage?
NoSQL DataBase

3. Describe the differences in scalability between a SQl and NoSQL database as though you were speaking to a non-technical friend.
SQL databases are relational, and NoSQL databases are non-relational.
SQL databases use structured query language (SQL) and have a predefined schema. NoSQL databases have dynamic schemas for unstructured data.
SQL databases are vertically scalable, while NoSQL databases are horizontally scalable.
SQL databases are table-based, while NoSQL databases are document, key-value, graph, or wide-column stores.
SQL databases are better for multi-row transactions, while NoSQL is better for unstructured data like documents or JSON.

# sql modeling techniques
1. Among data tables, what is a one-to-many relationship and how do we “relate” them?
it is a type of relationship where a single record in one table is associated with multiple records in another table we can relate them by using foreign keys that reference the primary key of the related table. 

2. Prior to designing your relational database, it might be useful to create a diagram of the database tables and their relationships.

3. Explain the difference between a primary and foreign key.
primary key is a identifier within a table, while a foreign key is a column that establishes relationships between tables by referencing the primary key of another table.

# SQL vs NoSQL

1. How do we treat keywords and parameters differently in SQL syntax?
Keywords must have predefined meanings and syntax, and they are interpreted by the SQL engine to perform specific operations.
Parameters act as placeholders for values that are supplied at runtime, allowing for dynamic and flexible query execution.

2. Define normalization within the context of schemas and data.
normalization is a fundamental concept in database design that promotes data integrity, eliminates redundancy, and improves the efficiency and effectiveness of data management and retrieval.

3. Explain the difference between one-to-one, one-to-many, and many-to-many relationships to a non-technical recruiter.
One-to-One: Unique pair, one entity corresponds to another.
One-to-Many: one entity relates to multiple instances of another entity.
Many-to-Many: multiple instances of one entity relate to multiple instances of another entity.

