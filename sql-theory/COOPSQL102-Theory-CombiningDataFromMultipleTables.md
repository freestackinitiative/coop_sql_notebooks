# Combining Data - Joins and multiple tables

If you feel confident in your understanding of joins, or you want to try some practical exercises first before diving into theory, skip ahead to the practice section in the SQL 102 Notebook. Otherwise, read on to learn about what joins are, why we use them, and how to include them in your queries.

### What are joins and why do we use them?

When we join data, we are merging two or more related tables into a single view, typically to add context to some analysis. This is accomplished by using common attributes (or *columns*) to establish relationships between the tables, along with constraints that control how records (or *rows*) are matched between them. There are four primary join types that each have their own affect on query results.

### A hypothetical join scenario

For example, let's say you have two tables, one with `company` data and another with `product` data. It would be useful to see a combined view of companies and their products for an analysis or report. 

To do this, we would join the `customer` and `product` tables together using a common field (or fields) that establish a relationship between them. In a relational database, this is generally done using a primary key/foreign key relationship. Then we would establish a constraint to determine how the rows should be matched between the two tables in the resulting query. The most common constraint is to specify that only matching values between the tables be included in the join (Ex: `A.column_a = B.column_a`). 

### Working through an example of the most common join - the `INNER JOIN`

Joins can be a difficult topic, so let's practice doing some together and then we'll explain what is happening as we go.

The first type of join we'll look at is the `INNER JOIN`. When we use an `INNER JOIN`, we are saying that we only want the values that match between the two tables based on our constraints. 

Let's assume we have two tables, `A` and `B`, that we want to join together, only including the records that are common to both tables. 

Here is what that query would look like:

**Query**
```SQL
SELECT
    A.column1,
    B.column1
FROM A -- This is the table on the "left-side" of the join
-- Specifying the join type
INNER JOIN B -- This is the table on the "right-side" of the join
-- Specifying the join column (`column1`) and constraint (`=`)
ON A.column1=B.column1 
```

This is a visual representation of which results will be returned between the two tables after the join:

**What gets matched between the two tables**

![Inner Join](https://www.codeproject.com/KB/database/Visual_SQL_Joins/INNER_JOIN.png)

As you can see, we're keeping only the results between the two tables that match based on our join columns and constraints. These results will only include those rows that matched and will drop data from both sides of the join that don't match. 

For the syntax of the join, we always specify the join type, column(s), and constraint(s) together. Joins come after the `FROM` clause and before the `WHERE` and `GROUP BY` clauses in our queries. 

To specify the type of join, we use the following general form: 

`{Join Type} {name of table to join}`

**Example:** `INNER JOIN company`

To specify the column and constraint, we use the following form:

`{First Table.Column to join on} {constraint} {Second Table.Column to join on}`

**Example:** `foods.company_id=company.company_id`

Putting it all together, writing the join would look like:

```SQL
INNER JOIN company
ON foods.company_id=order_details.company_id
```

>*Note: We typically use dot (`.`) notation when we join two or more tables in >SQL. This is so that we don’t confuse the SQL engine when two tables have >columns with the same name. Here’s the general syntax: `table_name.column_name`*

Overall, there are **four join types** that you should be aware of (and which we will cover):

- `INNER JOIN`: Only keep the records that match the constraint between the two tables

    ![Inner Join](../assets/inner-join-company-foods.png)

- `LEFT JOIN`: Keep all the records from the left-side of the join, and only show values for the records on the right-side that matched. Any values from the right-side that weren't matched will be assigned a `null` value.

    ![Left Join](../assets/left-join-company-foods.png)

- `RIGHT JOIN`: The opposite of the `LEFT JOIN` - keep all the records from the right-side of the join and only show values for the records on the left-side that matched. Any values from the left-sie that weren't matched will be assigned a `null` value.

    ![Right Join](../assets/right-join-company-foods.png)

- `FULL OUTER JOIN`: Keep all records between both tables, but only show the values that match my constraint. All other records that don't match will be included, but those values will be set to null.

    ![Full Outer Join](../assets/full-outer-join-company-foods.png)
    
We will dive a bit deeper into the details of each of these join types as we work through some practical examples in the SQL 102 Notebook. Also, these are only four join types out of many. There are some more advanced joins, like [cross-joins, natural joins, and self-joins](https://www.linkedin.com/pulse/what-difference-between-natural-joincross-join-self-madhu-mitha-k) that you should eventually become familiar with as you enhance your skills and understanding.

## Practical considerations for selecting attributes/columns for joins

Joining datasets usually depends on primary and foreign key relationships, but these aren't always clear (or available), especially with unfamiliar data. In such cases, understanding the data's origin, purpose, and contents can help. This can be done by finding documentation like data dictionaries or entity relationship diagrams (ERDs) or consulting with subject matter experts.

If there's no documentation or experts, exploratory data analysis becomes crucial. This involves understanding column data types, summary statistics, and identifying missing values. Aim to identify unique identifier columns, or potential primary keys for joins, which should be unique and non-null. [The information_schema](https://en.wikipedia.org/wiki/Information_schema), found in most relational databases, can also provide helpful metadata.

The last step in joining datasets is connecting tables using primary keys identified earlier. If key relationships are known, this is simple. Otherwise, analyze and understand primary keys, look for common columns, and try joining. Duplicates after joining suggest incorrect column usage. This illustrates why it is crucial for you to understand your data.