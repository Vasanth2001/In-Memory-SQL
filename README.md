# In-Memory-SQL
Designed and implemented a SQL-RDBMS in C/C++, focusing on internal design and SQL operations (SELECT, CREATE, INSERT, DELETE). Integrated algorithms for features like Aggregate functions, Joins, Where, Group by Clauses, and Nested Queries.

# Project Architecture Overview

1. B+ Tree Library: Utilized as a standard data structure for efficient data retrieval and management.Integrated into the RDBMS project with slight modifications to meet specific needs.

2. RDBMS Project SQL Interface: Responsible for parsing and validating SQL queries entered by users. Ensures that only valid queries are forwarded to the SQL engine. Facilitates interaction between the SQL engine and the B+ Tree Library

3. Mathematical Expression Library:  Manages expression trees, including creation, evaluation, optimization, and traversal. Used by the SQL engine to compute mathematical expressions embedded within SQL queries.

4. SQL Engine: Core component (pink portion) responsible for executing SQL queries. Utilizes the SQL interface to validate and process queries. Interfaces with the B+ Tree Library for CRUD operations on data. Utilizes the Mathematical Expression Library for computation of mathematical expressions.

5. SQL Interface:  APIs facilitating interaction between the SQL Engine and the Mathematical Expression Library. Developed incrementally to enhance integration and functionality as the project progresses.

# Supported Features
1. Storage Model: Records stored as tables, utilizing B+ trees for underlying data management.
2. Primary Keys: Support for defining primary keys in tables.
3. Supported SQL Queries: Basic support for SELECT, UPDATE, and DELETE queries.
4. Concurrency Control: Basic support for managing single-user concurrency.
5. Query Execution Plan: Implementation of a query execution plan.

# Conclusion
This project focuses on implementing a foundational SQL engine using the B+ tree data structure for in-memory record storage. By prioritizing essential functionalities like CRUD operations and basic query execution, the project provides practical experience in system programming and database management principles. Key components include the SQL interface, query execution plan, and integration with a B+ tree library. Exclusions such as advanced features (e.g., data integrity checks, ACID properties, indexing, persistence, and triggers) streamline development while offering opportunities for future enhancements. Upon completion, participants will have developed a functional single-user RDBMS capable of handling basic SQL queries. This project reinforces theoretical knowledge with practical application, preparing learners to expand their database management skills in subsequent courses or projects.
