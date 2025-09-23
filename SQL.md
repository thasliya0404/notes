# SQL 

* SQL = Structured Query Language.
* Used for storing, managing, and retrieving data in relational databases (RDBMS like MySQL, PostgreSQL, Oracle, SQL Server).

## Types of SQL Commands

* DDL (Data Definition Language) – Defines structure of database.
CREATE, ALTER, DROP, TRUNCATE, RENAME
* DML (Data Manipulation Language) – Manipulates data in tables.
INSERT, UPDATE, DELETE
* DQL (Data Query Language) – Query data.
SELECT
* DCL (Data Control Language) – Permissions.
GRANT, REVOKE
* TCL (Transaction Control Language) – Transactions.
COMMIT, ROLLBACK, SAVEPOINT

<img width="1280" height="778" alt="image" src="https://github.com/user-attachments/assets/bfeb8ba7-0ffa-4411-9804-0960887c5ed4" />

## Constraints

* PRIMARY KEY = unique + not null
* FOREIGN KEY = link to another table
* UNIQUE = no duplicate values
* NOT NULL = cannot store null
* CHECK = condition must be true
* DEFAULT = assign default value

## Joins

* INNER JOIN – common records in both tables
* LEFT JOIN – all from left + matching from right
* RIGHT JOIN – all from right + matching from left
* FULL OUTER JOIN – all from both tables
* SELF JOIN – join table with itself

## Clauses

* WHERE = filters rows
* GROUP BY = groups rows
* HAVING = condition after grouping
* ORDER BY = ascending/descending order
* LIMIT = restrict number of rows

## Aggregate Functions

* COUNT() = number of rows
* SUM() = total
* AVG() = average
* MIN() = smallest
* MAX() = largest

## Subqueries

Query inside another query.

## Views

Virtual table from a query.

## Indexes

Improves search speed.

## Transactions

Used for safe data handling.

## Importance of SQL in Data Analysis and Data Science

1. Foundation of Data Management:
* SQL is the standard language for managing and manipulating relational databases.
* It allows for efficient querying, updating, and managing of data stored in relational databases
2. Data Extraction:
* SOL enables the extraction of relevant data from large datasets.
* Analysts and data scientists use SQL to filter, aggregate, and transform data to gain insights
3. Data Manipulation:
* SOL allows for the creation, updating, and deletion of data records.
* It provides robust functions for data cleaning and preparation, which are crucial steps in data analysis
4. Integration with Data Tools:
* SQL integrates seamlessly with various data analysis and data science tools like R, Python (via libraries such as pandas, SQLAlchemy), and business intelligence tools (like Tableau, Power BI) It allows for easy data retrieval and  manipulation directly within these tools.
5. Handling Large Datasets:
* SQL is optimized for handling large volumes of data efficiently.
* It enables complex queries and operations on big data, which are common in data science projects
6. Data Aggregation and Summarization:
* SQL provides powerful functions for data aggregation, such as GROUP BY, SUM, AVG, COUNT, and more
* These functions are essential for summarizing data and performing statistical analysis.
7. Data Security and Integrity:
* SQL supports robust security features to protect sensitive data.
* It ensures data integrity through constraints, transactions, and normalization.
8. Support for Advanced Analytics:
* SQL can be used in conjunction with advanced analytical techniques, such as machine learning and predictive modeling.
* Data scientists can use SQL to preprocess data before feeding it into machine learning algorithms.
9. Real-time Data Processing:
* SQL is used in real-lime data processing and analytics through tools like Apache Kafka and Apache Flink
* It helps in monitoring and analyzing streaming data for real-time insights.


## Different types of Keys

* Primary key
* Foreign key
* Composite key
* Unique key

## Data types

* Char
* Varchar
* Int
* Boolean
* Float
* Date
* Datetime

## Database languages

* Data Definition Language
* Data Manipulation Language
* Data Control Language
* Transaction Control Language

## Basic SQL statements
<img width="1280" height="696" alt="image" src="https://github.com/user-attachments/assets/2b2e2337-9eed-482c-8ffb-692d79a5f58e" />













