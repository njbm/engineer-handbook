# 🧠 MySQL / Database Interview Questions & Answers

### Q1: What is the difference between `INNER JOIN` and `LEFT JOIN`?
- A: `INNER JOIN` returns rows with matching keys in both tables. `LEFT JOIN` returns all rows from the left table even if there’s no match.

### Q2: What is normalization?
- A: Organizing tables to reduce redundancy and improve data integrity.

### Q3: What are the normal forms?
- A:
  - 1NF: No repeating groups
  - 2NF: 1NF + no partial dependencies
  - 3NF: 2NF + no transitive dependencies
  - BCNF: Stronger version of 3NF

### Q4: What is an index?
- A: A database structure that improves query performance.

### Q5: When should you avoid using indexes?
- A: On low-cardinality or frequently updated columns.

### Q6: What is a foreign key?
- A: A column that links to the primary key of another table.

### Q7: What is ACID in databases?
- A: Atomicity, Consistency, Isolation, Durability.

### Q8: What are transactions?
- A: A group of operations executed together as a unit.

### Q9: Difference between `WHERE` and `HAVING`?
- A: `WHERE` filters before aggregation, `HAVING` filters after.

### Q10: `CHAR` vs `VARCHAR`?
- A: `CHAR` is fixed-length, `VARCHAR` is variable-length.

### Q11: What is a composite key?
- A: A primary key using multiple columns.

### Q12: What are stored procedures?
- A: Precompiled routines stored in the database.

### Q13: What is a view?
- A: A virtual table created from a query.

### Q14: `UNION` vs `UNION ALL`?
- A: `UNION` removes duplicates; `UNION ALL` keeps them.

### Q15: What is a subquery?
- A: A query inside another query.

### Q16: What is a surrogate key?
- A: A generated (e.g., auto-incremented) unique ID.

### Q17: How do indexes work?
- A: MySQL uses B-trees (or Hash for MEMORY engine).

### Q18: What is a clustered index?
- A: The table rows are stored in index order (InnoDB).

### Q19: What is a non-clustered index?
- A: An index stored separately from actual row data.

### Q20: What is query optimization?
- A: Improving performance using execution plans, indexes, etc.

### Q21: What does `EXPLAIN` do?
- A: Shows how MySQL executes a query.

### Q22: What is a self join?
- A: A table joined to itself.

### Q23: Common join types?
- A: INNER, LEFT, RIGHT, FULL OUTER, CROSS JOIN.

### Q24: What is referential integrity?
- A: Ensuring foreign key values always match primary keys.

### Q25: Many-to-many relationships?
- A: Achieved using a pivot/junction table.

### Q26: One-to-one relationship?
- A: One row in one table maps to one row in another.

### Q27: One-to-many relationship?
- A: One row maps to many rows in another table.

### Q28: What is a composite index?
- A: Index involving multiple columns.

### Q29: `DELETE` vs `TRUNCATE`?
- A: `DELETE` logs individual row deletions; `TRUNCATE` is faster and resets auto-increment.

### Q30: Primary key vs Unique key?
- A: Both enforce uniqueness, but only one PK per table.

### Q31: What is a trigger?
- A: Executes automatically on events like INSERT/UPDATE/DELETE.

### Q32: What is cascading?
- A: Automatic update/delete of child rows with parent changes.

### Q33: Use of `LIMIT`?
- A: Restrict number of rows returned.

### Q34: What is `OFFSET`?
- A: Skip rows before starting to return rows.

### Q35: What is a full-text index?
- A: Used for natural language text search.

### Q36: What are isolation levels?
- A: Control visibility of uncommitted data (Read Uncommitted → Serializable).

### Q37: Default isolation level in MySQL?
- A: REPEATABLE READ (InnoDB).

### Q38: Detecting slow queries?
- A: Enable slow query log or use Performance Schema.

### Q39: `UNION` vs `JOIN`?
- A: `UNION` merges rows vertically; `JOIN` merges columns.

### Q40: Temporary tables?
- A: Exist only during a session.

### Q41: Handling large datasets?
- A: Use pagination, indexing, caching, partitioning.

### Q42: What is a deadlock?
- A: Two transactions blocking each other.

### Q43: Foreign key constraints?
- A: Enforce valid links between parent and child tables.

### Q44: What is schema design?
- A: Structuring a database logically.

### Q45: What is denormalization?
- A: Intentionally introducing redundancy for performance.

### Q46: What is ENUM?
- A: Column type allowing a predefined set of values.

### Q47: What is NULL?
- A: Represents missing/unknown values.

### Q48: What is `COALESCE()`?
- A: Returns the first non-NULL value.

### Q49: What is `IFNULL()`?
- A: Returns fallback if value is NULL.

### Q50: Why use `IS NULL` instead of `= NULL`?
- A: `= NULL` is invalid; use `IS NULL` instead.
