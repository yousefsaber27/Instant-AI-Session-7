Database normalization is a process used to organize a database schema into tables and columns to reduce redundancy and dependency, ensuring data integrity. There are several normal forms (1NF, 2NF, 3NF, BCNF, 4NF, 5NF) that represent increasing levels of normalization. Here’s a summary of each and when to use them:

1. **First Normal Form (1NF)**:
   - Ensures that each column contains atomic (indivisible) values.
   - Use when you have repeating groups of data within a table.

2. **Second Normal Form (2NF)**:
   - Meets all the requirements of 1NF.
   - Removes partial dependencies, meaning no non-key attribute is dependent on only a portion of the primary key.
   - Use when a table has a composite primary key and non-key attributes depend on part of that key.

3. **Third Normal Form (3NF)**:
   - Meets all the requirements of 2NF.
   - Removes transitive dependencies, ensuring that no non-key attribute depends on another non-key attribute.
   - Use when you want to ensure data is free from redundancy and update anomalies.

4. **Boyce-Codd Normal Form (BCNF)**:
   - A stricter form of 3NF where every determinant (attribute that determines another) is a candidate key.
   - Use when you need to further minimize redundancy and ensure more efficient database design.

5. **Fourth Normal Form (4NF)**:
   - Addresses multi-valued dependencies where one or more independent multi-valued facts depend on the same primary key.
   - Use when dealing with complex relationships and to further reduce redundancy.

6. **Fifth Normal Form (5NF)**:
   - Deals with cases where a table contains join dependencies and ensures that it's free of join anomalies.
   - Use when you have complex relationships and need to maintain data integrity in very large databases.

**When to Use Database Normalization**:
- **Reduce Redundancy**: Normalization eliminates redundant data storage, which minimizes storage requirements and reduces the chance of inconsistencies.
  
- **Data Integrity**: By reducing redundancy and dependency, normalization helps maintain data integrity. Updates, inserts, and deletes are less likely to result in anomalies.

- **Query Optimization**: Normalization can lead to improved query performance by reducing the number of joins and making queries more straightforward.

- **Scalability**: Normalized databases are typically more scalable because they are easier to extend and modify without affecting existing data.

Normalization is typically applied during the database design phase to ensure that the database schema is well-structured, efficient, and capable of maintaining data integrity throughout its lifecycle.
