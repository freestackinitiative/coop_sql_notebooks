# COOP SQL Classes

## About these classes

Welcome to the new page for COOP Careers SQL Classes! You will find everything you need to follow along with the SQL content for the Data Analytics curriculum here. 

Here is a breakdown of the classes:
- [**SQL 101 - Introduction to Databases and Querying:**](#sql-101---introduction-to-databases-and-querying) Learn the foundational theory behind relational databases and SQL. Then apply that theory to learning how to write basic queries against single tables in a database.

- [**SQL 102 - Intermediate Queries and Combining Data:**](#sql-102---intermediate-queries-and-combining-data) Refine the querying skills that you began developing in SQL 101 and learn how to combine data from multiple tables using joins. You'll learn the theory behind how joins work and more advanced querying techniques. After completing this course, you will be better prepared for entry-level SQL technical interview questions.

- [**SQL Murder Mystery:**](#sql-murder-mystery) There's been a murder in SQL City and we need your SQL skills to help us find the killer! This is your chance to put the skills you learned in SQL 101 and 102 to the test and solve the mystery of who committed the murder in SQL City!

## How this works

Each class (SQL 101 & 102) has both a `Theory` section and a `Practice` section. In the theory section, you will read about fundamental concepts such as how databases work and how SQL works. Then, in the practical section, you will learn how to write queries to retrieve and analyze data from a database. 

You should start with the theory section first, then move on to the practice sections. The classes are structured so that the practice sections build on the theory we teach you with practical applications. The classes should also be done in order: start with the 101 theory section first - then do the practice section - before moving on to 102.

### Jupyter Notebooks - Our "Database Environment"

The practice section of each course is built using Jupyter Notebooks - a rich, multi-media document that enables you to mix narrative writing with code. This allows us to include written instruction alongside an environment that allows you to execute SQL queries against a database.

You will be connected to an actual RDBMS in these notebooks and will run your queries inside of the notebook. Instructions on how to run your queries are included in the first section of each notebook. To open the notebooks, simply click the ![Open in Colab Button](https://colab.research.google.com/assets/colab-badge.svg) button next to each notebook.

If you have never heard of a Jupyter Notebook and don't know how they work, we suggest you [watch this video first.](https://www.youtube.com/embed/eJDxcR1V7Qg?si=SRxRgxf7jPya-3Vd)


**SQL Cheatsheet**

We also recommend this [SQL Cheat Sheet](https://martinmarroyo.github.io/sqlcheatsheetandresources-coop/) to use as a companion to the notebooks and lessons. It was made the cheat sheet with the lesson content in SQL 101 and 102 in mind.

---

## **SQL 101 - Introduction to Databases and Querying**

**Theory Section:** [Introduction to Databases and Relational Databases](/sql-theory/COOPSQL101-Theory-IntrotoDatabasesandRelationalDatabases.md)

**Practice Section - Basic Data Retrieval Notebook:** <a target="_blank" href="https://colab.research.google.com/github/freestackinitiative/coop_sql_notebooks/blob/2.0/COOP_SQL_101_PracticeNotebook.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>  

Topics Covered:

- Selecting data (`SELECT`)
- Filtering data (`WHERE`/`HAVING`)
- Sorting data (`ORDER BY`)
- Aggregating/Summarizing data (`GROUP BY`, `AVG`, `COUNT`, `SUM`)

---

## **SQL 102 - Intermediate Queries and Combining Data** 

**Theory Section:** [Combining Data From Multiple Tables](sql-theory/COOPSQL102-Theory-CombiningDataFromMultipleTables.md) 

**Practice Section - Intermediate Queries Notebook:** <a target="_blank" href="https://colab.research.google.com/github/freestackinitiative/coop_sql_notebooks/blob/main/COOP_SQL_102.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

Topics Covered:

- Combining Data (`INNER`, `LEFT`, `RIGHT`, `FULL OUTER` joins)
- Intermediate Queries and Scalar functions (Using the `CASE` statement, `ROUND`, `DATEDIFF`, etc.)
- Subqueries & Common Table Expressions (CTE)
- Window/Analytical functions (`ROW_NUMBER`, `RANK`, `DENSE RANK`)

--- 

## **SQL Murder Mystery** 

**SQL Murder Mystery Notebook:** <a target="_blank" href="https://colab.research.google.com/github/freestackinitiative/coop_sql_notebooks/blob/main/COOP_SQL_Murder_Mystery.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

A murder happened in SQL City, and we need your SQL skills to help crack the case! Put the skills that you learned in SQL 101 and 102 to the test and solve the SQL Murder Mystery!

Topics Covered:

- Everything in SQL 101 & 102!