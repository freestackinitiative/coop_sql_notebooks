# COOP SQL Classes

## About these classes

Welcome to COOP Careers SQL Classes! You will find everything you need to follow along with the SQL content for the Data Analytics curriculum here. 

Our classes can be broken down into two sections: **Theory** and **Practice**. The theory classes are crash courses on things you should know to understand how databases work, as well as how to use SQL. The practice classes are where you will get hands-on practice to develop your querying skills and complete your labs - it's the main material that your captains will use to teach SQL 101 - 103.

**Theory (Asynchronous)**

- [**SQL 100 - Introduction to Relational Databases and SQL**](#sql-100---introduction-to-relational-databases-and-sql) Learn the foundational theory behind relational databases and SQL. This crash course gives you the highlights from a university course in Databases that you should know in about 30 minutes. Go through this before completing `SQL 101`.
- [**SQL 103A - Combining Data in SQL: How to use `JOIN` and `UNION`**](#sql-103a---combining-data-in-sql-how-to-use-join-and-union) A primer on how to combine data horizontally (using `JOIN` statements) and vertically (using `UNION`). You can use this to learn how joins work and as a refresher before SQL interviews. ***Read this before you take SQL 103.*** 

  >**Prerequisite**: You should have already gone through at least SQL 100 and SQL 101 before doing this.

**Practice**

- [**SQL 101 - Basic Data Retrieval:**](#sql-101---basic-data-retrieval)  Apply the theory you learned in the Database Crash Course to learning how to write basic queries against single tables in a database.
- [**SQL 102 - Advanced Querying Techniques:**](#sql-102---advanced-querying-techniques) Refine the querying skills that you began developing in SQL 101 and learn advanced techniques to write more complex queries and improve your search results. Here you'll learn about using the `CASE` statement to add search conditions to your queries, basic scalar functions, how to use subqueries and common table expressions (CTEs) for multi-step queries. With these techniques in your toolkit, you'll be able to write queries that answer more complex questions that are more likely to come up on the job.  
- [**SQL 103 - Combining Data from Multiple Tables:**](#sql-103---combining-data-from-multiple-tables) Up to this point, you have only written queries that deal with a single table. But many real-world scenarios will require you to combine data from multiple tables to answer questions. Here, we'll teach you how to combine data from multiple tables using `joins`. You'll learn the theory behind how joins work, the different methods of joining data, and when to use each one. After completing this course, you will be better prepared for entry-level SQL technical interview questions.
- [**SQL 104 - SQL Murder Mystery:**](#sql-murder-mystery) There's been a murder in SQL City and we need your SQL skills to help us find the killer! This is your chance to put the skills you learned in SQL 101 to 103 to the test and solve the mystery of who committed the murder in SQL City!

## How this works

For most students, the following path through these courses is recommended:
1. SQL 100 - Introduction to Relational Databases and SQL (*~30 minutes to complete*)
2. SQL 101 - Basic Data Retrieval (*~2.5 hours to complete*)
3. SQL 102 - Advanced Querying Techniques (*~2 hours to complete*)
4. SQL 103A - Combining Data in SQL: How to use `JOIN` and `UNION` (*~30 minutes to complete*)
5. SQL 103 - Combining Data from Multiple Tables (*~2.5 hours to complete*)
6. SQL 104 - SQL Murder Mystery

The theory courses (1 & 4) will be assigned as pre-reading homework before the SQL 101 and 103 classes, respectively. You will work on SQL 101, 102, and 103 (2, 3, 5) with your captains in class. Then, you will have a week to solve the SQL Murder Mystery (6) independently. 

### Jupyter Notebooks - Our "Database Environment"

The practice section of each course is built using Jupyter Notebooks - a rich, multi-media document that enables you to mix narrative writing with code. This allows us to include written instruction alongside an environment that allows you to execute SQL queries against a database.

You will be connected to an actual RDBMS in these notebooks and will run your queries inside of the notebook. Instructions on how to run your queries are included in the first section of each notebook. To open the notebooks, simply click the ![Open in Colab Button](https://colab.research.google.com/assets/colab-badge.svg) button next to each notebook.

If you have never heard of a Jupyter Notebook and don't know how they work, we suggest you [watch this video first.](https://www.youtube.com/embed/eJDxcR1V7Qg?si=SRxRgxf7jPya-3Vd)


**SQL Cheatsheet**

We also recommend this [SQL Cheat Sheet](https://martinmarroyo.github.io/sqlcheatsheetandresources-coop/) to use as a companion to the notebooks and lessons. The cheat sheet was made with the lesson content in SQL 101, 102, and 103 in mind.

---

## **Classes**

### **SQL 100 - Introduction to Relational Databases and SQL** 

[**Click Here**](/sql-theory/COOPSQL101-Theory-IntrotoDatabasesandRelationalDatabases.md) to access the Database Crash Course.

- **Slide Deck**: [Click Here](https://docs.google.com/presentation/d/1kK4vbOvCt8N2Xg9Zqht1JmssDZkESJDbZzJlYkolsTo/edit?usp=sharing)
- **Lecture Video**: [Click Here](https://drive.google.com/file/d/1NVmCvai1odVcW0omK7AKaB0AvE69Q2gZ/view)

[Back to top](#about-these-classes)

---

### **SQL 101 - Basic Data Retrieval**

**SQL 101 Notebook:** <a target="_blank" href="https://colab.research.google.com/github/freestackinitiative/coop_sql_notebooks/blob/main/notebooks/COOP_SQL_101_PracticeNotebook.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>  

**SQL 101 Slide Deck:** [Click Here](https://docs.google.com/presentation/d/1K0oZEydysFZJaclFJcMPy-SsYBg2X2yI9yi8TCTAZ3U/edit?usp=sharing)

Topics Covered:

- Selecting data (`SELECT`)
- Filtering data (`WHERE`/`HAVING`)
- Aggregating/Summarizing data (`GROUP BY`, `AVG`, `COUNT`, `SUM`)
- Sorting data (`ORDER BY`)

[Back to top](#about-these-classes)

---

### **SQL 102 - Advanced Querying Techniques** 

**SQL 102 Notebook:** <a target="_blank" href="https://colab.research.google.com/github/freestackinitiative/coop_sql_notebooks/blob/main/notebooks/COOP_SQL_102_PracticeNotebook.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

**SQL 102 Slide Deck:** [Click Here](https://docs.google.com/presentation/d/1wmNuyjT7Z6QLrEBJMZRXx2FZ6fXnfmtmhRAa-dc92t4/edit?usp=sharing)

Topics Covered:

- `CASE` Statements
- Scalar functions
- Subqueries 
- Common Table Expressions (CTE)

[Back to top](#about-these-classes)

--- 

### **SQL 103A - Combining Data in SQL: How to use `JOIN` and `UNION`**

[**Click Here**](sql-theory/COOPSQL103-Theory-CombiningDataFromMultipleTables.md) to access SQL 103A. 

- [**Lecture Video**]()

[Back to top](#about-these-classes)

---
### **SQL 103 - Combining Data from Multiple Tables**

**SQL 103 Notebook:** <a target="_blank" href="https://colab.research.google.com/github/freestackinitiative/coop_sql_notebooks/blob/main/notebooks/COOP_SQL_103_PracticeNotebook.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>

**SQL 103 Slide Deck:** [Click Here](https://docs.google.com/presentation/d/15PczTO_7yZ97QaMjPKUosRUBa9Hw5G_oAgX1hDlfzdc/edit?usp=sharing)

Topics Covered:
- `JOIN`s (`INNER`, `LEFT`, `RIGHT`, `FULL OUTER`)
- `UNION`

[Back to top](#about-these-classes)

---

### **SQL 104 - SQL Murder Mystery** 

**SQL Murder Mystery Notebook:** <a target="_blank" href="https://colab.research.google.com/github/freestackinitiative/coop_sql_notebooks/blob/main/notebooks/COOP_SQL_Murder_Mystery.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

A murder happened in SQL City, and we need your SQL skills to help crack the case! Put the skills that you learned in SQL 101 - 103 to the test and solve the SQL Murder Mystery!

Topics Covered:

- Everything in SQL 101, 102, and 103!

[Back to top](#about-these-classes)