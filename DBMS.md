# 100 DBMS Interview Questions with Answers

## Basic Concepts

1. **What is a Database Management System (DBMS)?**
A DBMS is software that enables users to define, create, maintain, and control access to databases. It facilitates storage, retrieval, modification, and deletion of data from databases efficiently and securely.
2. **What are the advantages of using a DBMS?**

- Improved data sharing and security
- Reduced data redundancy and inconsistency
- Enhanced data integrity
- Backup and recovery mechanisms
- Concurrent access for multiple users
- Easier data access through queries

3. **What is a database?**
A database is an organized collection of related data stored in a structured format, typically in tables, to facilitate efficient retrieval and management.
4. **Difference between a DBMS and a file system?**
A DBMS manages data centrally and supports features like data integrity, security, and multi-user access; a file system just stores raw files and lacks these features.
5. **What is a relational database?**
It organizes data into tables (relations) of rows and columns where each row is a record and each column a field.
6. **Explain Data Independence.**
Data independence refers to the capacity to change the schema at one level of a database system without affecting the schema at the next higher level.
7. **What is a primary key?**
A primary key is a field or combination of fields that uniquely identifies each record in a table.
8. **What is a foreign key?**
A foreign key is a field in one table that refers to the primary key in another table, establishing a relationship between the tables.
9. **What is normalization?**
Normalization is the process of organizing data to reduce redundancy and improve data integrity by dividing large tables into smaller, related tables.
10. **What are denormalization and its purpose?**
Denormalization is the process of combining tables to improve read performance at the expense of some redundancy.

## Database Architecture

11. **What are the different types of DBMS architectures?**

- Single-tier
- Two-tier (client-server)
- Three-tier (client, application server, database server)

12. **Difference between two-tier and three-tier architectures?**
A two-tier architecture connects the client directly to the database server; a three-tier architecture adds an application server between the client and the database for scalability and security.
13. **Explain schema and instance in DBMS.**
Schema is the design structure of a database; instance is the data stored in the database at a particular moment.
14. **What is data abstraction?**
It is the process of hiding implementation details and showing only necessary features of data to the user.
15. **What are the levels of data abstraction?**

- Physical Level: How data is stored
- Logical Level: What data is stored and relationships
- View Level: Part of the database the user interacts with


## Data Models

16. **What are data models in DBMS?**
Data models define how data is connected, stored, and manipulated. Examples include Hierarchical, Network, Relational, and Object-oriented models.
17. **What is the Entity-Relationship (ER) Model?**
An ER Model represents real-world entities and their relationships in a diagrammatic form using entities, attributes, and relationships.
18. **Difference between entity and attribute.**
An entity is an object with a distinct existence; an attribute is a property describing the entity.
19. **What is a relationship in DBMS?**
A connection or association between two or more entities.
20. **Explain cardinality in ER models.**
Cardinality is the number of instances of one entity that relate to the number of instances in another entity.

## Keys and Constraints

21. **List and explain different types of keys.**

- Super Key: Any combination of columns that uniquely identifies a row
- Candidate Key: Minimal super key
- Primary Key: Chosen candidate key
- Unique Key: Ensures all values are unique
- Foreign Key: References primary key of another table
- Composite Key: More than one attribute to identify rows

22. **What are integrity constraints?**
Rules that ensure data integrity in the database, such as primary key, foreign key, unique, not null, and check constraints.
23. **What is a unique key?**
A constraint that ensures all values in a column or a set of columns are unique across rows in a table.
24. **Can a table have multiple primary keys?**
No; a table can have only one primary key but may have multiple unique keys.
25. **Difference between primary key and candidate key.**
All candidate keys can uniquely identify records; the primary key is the chosen candidate key used for identification.

## SQL and Query

26. **What are the main types of SQL statements?**

- DDL (Data Definition Language): CREATE, ALTER, DROP
- DML (Data Manipulation Language): SELECT, INSERT, UPDATE, DELETE
- DCL (Data Control Language): GRANT, REVOKE
- TCL (Transaction Control Language): COMMIT, ROLLBACK, SAVEPOINT

27. **What is a join? List its types.**
A SQL operation to combine rows from two or more tables based on a related column. Types: INNER JOIN, LEFT JOIN, RIGHT JOIN, FULL JOIN, CROSS JOIN.
28. **Difference between INNER JOIN and LEFT JOIN.**
INNER JOIN returns records common to both tables; LEFT JOIN returns all records from the left table and matched ones from the right, with NULLs for no matches.
29. **What is a subquery?**
A query nested within another query.
30. **What is a view?**
A virtual table based on the result set of a SQL query.

## Advanced SQL

31. **What are stored procedures?**
Precompiled collection of SQL statements stored under a name, which can be executed as a program.
32. **What are triggers?**
Procedures that execute automatically in response to certain events on a table or view (e.g., INSERT, UPDATE, DELETE).
33. **What is an index? Types?**
An index is a data structure that improves the speed of data retrieval. Types: clustered, non-clustered, unique, and composite.
34. **Difference between cluster and non-clustered index.**
A clustered index sorts and stores data rows in the table; non-clustered index stores a pointer to the data.
35. **What is a cursor in SQL?**
A database object used to retrieve, manipulate, and navigate rows in a result set one at a time.

## Normalization

36. **What is First Normal Form (1NF)?**
A table is in 1NF if it contains only atomic (indivisible) values and each column contains only one value per row.
37. **Explain Second Normal Form (2NF).**
A table is in 2NF if it is in 1NF and all non-key attributes are fully dependent on the primary key.
38. **What is Third Normal Form (3NF)?**
A table is in 3NF if it is in 2NF and all non-key attributes are non-transitively dependent on the primary key.
39. **What is Boyce-Codd Normal Form (BCNF)?**
A stricter version of 3NF where every determinant is a candidate key.
40. **What is a partial dependency?**
When a non-key attribute is dependent on part of a composite primary key, not the whole key.

## Transactions

41. **What is a transaction?**
A sequence of operations performed as a single logical unit of work, which must be completed in its entirety or not at all.
42. **What are ACID properties?**

- Atomicity: All or nothing
- Consistency: Maintains database correctness
- Isolation: Transactions are isolated
- Durability: Changes persist after commit

43. **What is a savepoint?**
A marker within a transaction that allows a partial rollback to that point.
44. **What is a commit?**
A command to permanently save all changes made during the transaction.
45. **What is a rollback?**
A command to undo changes made in a transaction up to the last commit or savepoint.

## Concurrency and Locking

46. **What is concurrency control?**
Techniques to ensure correct results for users when multiple transactions execute concurrently.
47. **What is locking in DBMS?**
A method to prevent multiple users from modifying the same data simultaneously.
48. **Types of locks in DBMS?**

- Shared Lock (read lock)
- Exclusive Lock (write lock)

49. **What is a deadlock?**
A situation where two or more transactions wait indefinitely for resources locked by each other.
50. **How can deadlocks be prevented?**
By resource ordering, avoiding circular wait, or using timeout mechanisms.

## Indexing and Optimization

51. **Why are indexes important?**
They speed up data retrieval operations at the expense of additional disk storage and slower updates.
52. **What is query optimization?**
The process of choosing the most efficient way to execute a SQL query.
53. **What is an execution plan?**
A visual or textual description of the steps the database engine will use to execute a query.
54. **What is a full table scan?**
Processing all the rows in a table to find matching results.
55. **What is an index scan?**
Searching the index data structure to locate data rows quickly.

## Backup and Recovery

56. **What is database backup?**
A process of creating a copy of the database to restore it in case of failure or loss.
57. **What are types of database backup?**

- Full backup
- Incremental backup
- Differential backup

58. **What is database recovery?**
The process of restoring a database to a correct state after failure.
59. **What is a checkpoint in DBMS?**
A point of synchronization between the database and the transaction log.
60. **How can data loss be minimized in DBMS?**
Through regular backups, replication, and transaction logs.

## Data Integrity and Security

61. **What is data integrity?**
The accuracy and consistency of data over its entire lifecycle.
62. **How does DBMS ensure data integrity?**
Through integrity constraints, transactions, and ACID properties.
63. **Types of integrity constraints?**

- Domain constraints
- Entity integrity
- Referential integrity
- User-defined constraints

64. **What is user authentication in DBMS?**
Verifying the identity of users accessing the database.
65. **What is authorization?**
Assigning specific permissions to users for accessing or manipulating data.

## Performance and Tuning

66. **What causes slow database performance?**

- Missing indexes
- Poorly written queries
- Insufficient hardware resources
- Lock contention
- Fragmentation

67. **How can database performance be improved?**

- Using proper indexes
- Optimizing queries
- Normalizing tables
- Partitioning data
- Regular maintenance

68. **What is partitioning?**
Dividing large tables into smaller, manageable pieces for improved performance.
69. **What is sharding?**
Horizontal partitioning of data across multiple databases or servers.
70. **What is replication in DBMS?**
Creating and maintaining copies of data across multiple locations.

## Advanced Topics

71. **What is normalization’s impact on performance?**
Normalization reduces redundancy and improves consistency, but excessive normalization may result in more complex queries and joins.
72. **What is denormalization’s impact on performance?**
Denormalization improves read performance by reducing the need for joins but may increase redundancy.
73. **What is materialized view?**
A database object that contains the results of a query and stores them physically for faster access.
74. **Difference between a View and a Materialized View.**
A view is virtual (no data stored); a materialized view stores the data.
75. **What is a surrogate key?**
A unique identifier for an entity, often automatically generated and has no business meaning.

## Design and Modeling

76. **What is database schema?**
A blueprint that defines how data is organized in a database.
77. **Difference between logical and physical data models.**
Logical data model defines the structure and relationships; physical data model defines how the data is stored.
78. **What is normalization vs. ER modeling?**
Normalization structures tables to remove redundancy; ER modeling captures the relationships and entities.
79. **What is a weak entity?**
An entity that cannot be uniquely identified by its attributes alone and relies on a foreign key.
80. **What is generalization and specialization in ER modeling?**
Generalization groups similar entities; specialization divides an entity set into sub-entities.

## Miscellaneous Questions

81. **What are system tables?**
Database tables that store metadata about the database structure, users, permissions, etc.
82. **What is data mining?**
Extracting useful patterns and insights from large sets of data.
83. **What is OLTP?**
Online Transaction Processing – handling large numbers of short, transactional queries.
84. **What is OLAP?**
Online Analytical Processing – supporting complex queries for data analysis.
85. **Difference between OLTP and OLAP?**
OLTP focuses on transactional tasks; OLAP supports data analysis and reporting.
86. **What is a NoSQL database?**
A database that provides a mechanism for storage and retrieval of data other than tabular relations used in relational databases.
87. **Types of NoSQL databases?**

- Document-based
- Key-value stores
- Column-family stores
- Graph databases

88. **Difference between SQL and NoSQL?**
SQL is structured, schema-based, relational; NoSQL is flexible, schema-less, and supports a variety of data models.
89. **What is polyglot persistence?**
Using different data storage technologies for different data needs within the same application.
90. **What is an object-oriented database?**
A database that stores data as objects, as used in object-oriented programming.

## Practical and Scenario-Based

91. **How do you find and fix slow queries?**
By analyzing query execution plans, indexing relevant columns, rewriting queries for efficiency, and using database performance tools.
92. **How do you restore a corrupted database?**
By using backup files and logs to restore the database to a consistent state.
93. **How do you migrate data from one DBMS to another?**
Exporting data, transforming schemas as needed, and importing data into the target DBMS.
94. **How can you ensure high availability in a database?**
Through replication, clustering, backup strategies, and failover mechanisms.
95. **Describe the process for a database upgrade.**
Back up the database, test the upgrade process on a staging environment, apply the upgrade, test for breakages, and go live.
96. **How do you secure sensitive data in DBMS?**
Encrypt data at rest and in transit, restrict user access, mask sensitive data, audit accesses.
97. **How do you handle large volumes of data in DBMS?**
Partition tables, use scalable storage, optimize queries, and possibly use distributed databases.
98. **How do you handle schema changes in a live system?**
Use migrations with scripts, take backups, schedule maintenance windows, communicate with users.
99. **Describe a scenario where normalization was essential.**
In customer data management, normalization helped reduce data redundancy and avoided update anomalies.
100. **Describe a scenario where denormalization was required.**
In a reporting system, denormalization improved query speed for large reports by reducing the need for joins.