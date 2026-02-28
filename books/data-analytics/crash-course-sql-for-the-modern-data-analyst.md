# Crash Course SQL for the Modern Data Analyst

**Author:** Minerva Technologies  
**Format:** PDF  
**Category:** data-analytics

---

## Page 2

s
Table Of Contents
Introduction
Chapter 1: Foundations of SQL
Chapter 2: Basic SQL Commands
Chapter 3: Advanced SQL Commands
Chapter 4: Common Real-World SQL Issues (Working with Timestamps)
Chapter 5: Common Real-World SQL Issues (Working with JSON Data)
Chapter 6: Common Real-World SQL Issues (Cleaning String Data)
Chapter 7: Common Real-World SQL Issues (Working with Arrays)

---

## Page 3

Chapter 8: Common SQL Technical Interview Questions
Chapter 9: Moving Forward
Introduction
The Power of Data
In today's digital age, data is often called the "new oil." It drives
decisions, shapes strategies, and offers previously unimaginable
insights. Data applications vary, from predicting consumer behaviour
to optimising supply chains. But raw data, in its unprocessed form, is
like crude oil—it needs refining to unlock its true potential. That is
where SQL comes into play.
What is SQL?
SQL, or Structured Query Language, is the standard language for
managing and querying data in relational databases. It allows users
to interact with data, retrieve specific information, and perform
complex operations, all with simple commands. For data analysts,
SQL is an indispensable tool. It is the bridge between raw data and
meaningful insights.

---

## Page 4

SQL in Action: Real-World Examples
E-commerce: Imagine an online store wanting to identify its
top 10 best-selling products in the last month. With SQL, a
simple query can retrieve this information from millions of
transaction records in seconds.
Healthcare: Hospitals can use SQL to analyse patient data,
identifying trends like the most common ailments in a
particular season or the average duration of hospital stays.
Finance: Investment banks might use SQL to analyse
trading data, identifying which stocks have the highest
trading volumes or which sectors see the most activity.
Social Media: Platforms like Twitter or Facebook can use
SQL to fetch user data, analyse trends, or even identify
viral content by querying the number of shares or likes.
Why SQL for Data Analysts?
Data analysts are the detectives of the digital world. They sift
through data to uncover patterns, draw conclusions, and provide
actionable insights. While there are many tools and languages
available for data analysis, SQL stands out for several reasons:
Universality: SQL is used by a vast majority of relational
database systems. Whether you are working with MySQL,
PostgreSQL, Oracle, or any other RDBMS, the
foundational concepts of SQL remain consistent.
Efficiency: SQL is designed to handle large datasets.
Complex operations that might take hours in other
languages can be executed in minutes with a well-crafted
SQL query.
Integration: SQL integrates seamlessly with other tools and
platforms. Whether visualising data in Tableau, performing
statistical analysis in R, or building machine learning
models in Python, SQL is often the starting point.
Navigating This Book

---

## Page 5

This eBook is designed as a crash course, taking you from the
basics of SQL to more advanced topics tailored for the data analyst
role. You'll find practical exercises to test your knowledge and
interview questions to prepare you for professional challenges.
Whether you are an aspiring data analyst, a professional looking to
upskill, or just curious about the world of data, this book is your
guide.
Let us embark on this journey to unlock the power of data with SQL!
Preparing Your SQL Workspace (Optional)
Having a relational database system at your disposal is beneficial to
learn and practice SQL effectively. Several freely available options
exist, including SQLite, MySQL, and PostgreSQL. SQLite is
recommended for beginners and those looking for a straightforward
experience due to its user-friendly nature and minimal setup
requirements.
Download and install SQLite.
Create a new database.
Connect to your database using an SQL client.
Please note: This book will not delve deeply into the setup process,
as it is designed assuming readers already have an SQL
environment ready. Our primary focus will be SQL commands,
syntax, and practical applications.

---

## Page 6

Chapter 1: Foundations of SQL
Understanding Databases and Tables
A relational database is like a well-organised filing cabinet. Imagine
you have several folders, each containing sheets of paper. Each

---

## Page 7

folder represents a table, and each sheet of paper inside it
represents a record. The details written on these sheets (like name,
age, and address) represent the data.
In technical terms, a relational database organises data into tables
(or "relations"). These tables are linked based on relationships,
ensuring data integrity and accuracy.
Basic SQL Syntax and Structure
SQL is like the language of databases. Just as we communicate in
English or any other language, databases understand SQL. Every
command or query you write in SQL gives specific instructions to the
database.
Every SQL query requires the following two clauses to run, namely
the SELECT and FROM.
For instance, if you want to retrieve all data from a table named
'Students', you would write:
Here:
SELECT tells the database what you want to do (in this
case, select or retrieve data).
The asterisk'*' is a wildcard character that means
"everything."
FROM Students, specify from which table you want to
retrieve the data.
To illustrate this further, let us consider a sample 'Students' table:

---

## Page 8

When you run the SELECT * FROM Students; query on this table,
you'll retrieve all the rows and columns, displaying the entire table as
shown above.
If you wanted to retrieve only the names of the students, you would
modify the query to:
Thus returning:
Data Types in SQL
In the real world, we have categories for data (like numbers, text,
and dates). In SQL, we have data types. These data types help the
database understand what information is stored and how to store it
efficiently.
Some common data types in SQL are:
INTEGER: For whole numbers (e.g., 1, 100, -30).
TEXT: For alphanumeric characters (e.g., "John", "A123").
REAL: For decimal numbers (e.g., 3.14, -0.001).

---

## Page 9

DATE: For dates (e.g., "2023-10-20").
For example, if you have a table 'Books' and you want to store the
title (as text) and publication year (as an integer), the structure might
look something like this:
Understanding data types is also crucial, as certain functions only
work on specific data types. For instance, you cannot add or
subtract values in a TEXT column but with INTEGER or REAL
columns. Similarly, date functions, which can help you extract the
month or year from a date, will only work on DATE data types.
Additionally, using the correct data type can save storage space. For
example, using an INTEGER for a phone number might seem
logical. Still, since phone numbers don't require mathematical
operations and can start with a zero, TEXT would be a more
appropriate choice.
A point to note, apart from these common data types, other types of
data do exist as well, such as:
JSON (JavaScript Object Notation) is a lightweight data-
interchange format that is easy for humans to read and
write and for machines to parse and generate.
Imagine you have a table named 'Users' and want to store user
preferences in a JSON format. The table might look something like
this:

---

## Page 10

ARRAY: An ARRAY data type can store a list of values in
a single column.
Imagine you have a table named 'Articles', and you want to store
tags associated with each article. The table might look like this:
BLOB (Binary Large Object): BLOBs store extensive
binary data, such as images or files.
Imagine you have a table named 'ProfilePics' where you store user
profile pictures:

---

## Page 11

Chapter 2: Basic SQL Commands
SELECT: Retrieving Data
We have showcased some examples of the SELECT command in
the previous chapter, but for a refresher, let us delve deeper into its
versatility and power. The SELECT command is not just about
retrieving data but also the correct data.
With the right combinations and conditions, you can tailor your
queries to extract precise information, be it a single column, multiple
columns, or even specific rows that meet certain criteria.
This command is the foundation of SQL, and mastering it is akin to
having a sharp tool in your data analysis toolkit. Whether looking for
a specific record, summarising data, or preparing a report, the
SELECT command is your starting point.
In the upcoming sections, we will explore advanced uses,
combinations, and tricks to make the most out of this essential SQL
command.
Imagine a table named 'Books' with columns 'Title', 'Author', and
'YearPublished'.

---

## Page 12

To view only the titles of the books, you would use:
WHERE: Filtering Data
The WHERE clause acts like a sieve or filter. Imagine you have a
bag of mixed candies and only want the red ones. You would sift
through the bag to pick them out. Similarly, the WHERE clause filters
out specific rows based on your set condition.
Using the 'Books' table, if you want to find books published in 2022,
you would use:
Numerical Comparison Operators
Comparison operators are used to compare one expression with
another. The result of a comparison is always a Boolean value that
can be true, false, or unknown. Examples of such operators include:
= (Equal to)
!= or <> (Not equal to)

---

## Page 13

(Greater than)
< (Less than)
>= (Greater than or equal to)
<= (Less than or equal to)
Imagine a table named 'Books' with a column 'Price'. To find books
priced at $20, you would use:
Logical Operators
Logical operators are used to combine two or more conditions.
They return true or false based on the conditions' results.
AND: Both conditions must be true.
OR: At least one condition must be true.
NOT: Negates the condition.

---

## Page 14

Using the 'Books' table, to find books priced between $10 and $20,
you would use:
LIKE
The LIKE operator searches for a specified pattern in a column. It is
often used with wildcard characters % (represents zero, one, or
multiple characters) and _ (represents a single character).
To find books with titles starting with "SQL", you would use:

---

## Page 15

Finding titles that have "to" somewhere in the name
Finding titles that have exactly one character between "o" and "D"
Finding titles that end with "Design"
OR
The OR operator filters records based on at least one of the
conditions being met and used to combine multiple conditions in a

---

## Page 16

WHERE clause, where at least one condition must be true.
To find books written by "John Doe" or priced above $25, you'd use:
IN
The IN operator allows you to specify multiple values in a WHERE
clause. It is a shorthand for multiple OR conditions.
To find books published in 2021 or 2023, you would use:

---

## Page 17

BETWEEN
The BETWEEN operator selects values within a given range. The
values can be numbers, text, or dates.
To find books priced between $20 and $30, you would use:
IS NULL

---

## Page 18

The IS NULL operator is used to test for empty values. It is typically
used to filter results based on null or missing values.
To find books without a review, you would use:
AND
The AND operator filters records based on multiple conditions in a
WHERE clause.

---

## Page 19

To find books written by "John Doe" and priced above $15, you
would use:
NOT
The NOT operator filters out records that meet a particular condition.
To find books not written by "John Doe", you would use:
ORDER BY: Sorting Data

---

## Page 20

Think of the ORDER BY clause as organising books on a shelf. You
can arrange them alphabetically, by size, or by publication date.
Similarly, ORDER BY arranges your data in a specific order, either
ascending (ASC) or descending (DESC).
Data will be sorted ascending by default, but with the DESC
keyword, you can reverse this order. Just as you might prefer to
have your favourite books at eye level or your most-referenced
materials at arm's reach, the ORDER BY clause allows you to
prioritise and present your data in a way that is most meaningful and
accessible.
For instance, examining sales data, you might want to see the most
recent transactions first. Or, if you are looking at a list of products,
you might want to sort them by price, from lowest to highest.
Using the reference table to list books in the order they were
published:
LIMIT: Restricting the Number of Rows Returned
The LIMIT clause restricts the number of rows returned by a query. It
is handy when dealing with large datasets where you only need a
subset of the results, such as paginating results on a website.

---

## Page 21

Using the 'Books' table, retrieve the first three books:
DISTINCT: Removing Duplicate Rows
The DISTINCT clause is used to remove duplicate rows from the
result set. It ensures the query returns unique values for the
specified column(s).
Using the 'Books' table, retrieve a list of unique authors:

---

## Page 22

INSERT, UPDATE, DELETE: Manipulating Data
These clauses allow you to manipulate data inside an existing data
table. Depending on the dependencies of the data table, sometimes
organisations have dedicated data engineers maintaining the
pipeline of the data instead of the analyst having to update it.
Nonetheless, analysts need to understand these commands, as they
might need to make temporary changes or work on smaller datasets
for specific projects. Moreover, knowing these commands equips an
analyst with the ability to troubleshoot data issues, collaborate
effectively with data engineers, and ensure data integrity.
In some scenarios, especially in smaller organisations or during the
initial stages of data setup, analysts might be required to handle data
manipulations directly. Thus, mastering these commands enhances
an analyst's skill set and provides flexibility in managing various data
scenarios.
These commands are like actions you take with physical items:
INSERT is like adding a new book to a shelf.

---

## Page 23

UPDATE is like replacing an old edition of a book with a
new one.
DELETE is like removing a book from the shelf.

---

## Page 25

Chapter 3: Advanced SQL Commands
JOIN Operations: Combining Tables (INNER JOIN)
The JOIN operation allows you to combine rows from two or more
tables based on a related column between them. There are several
types of JOINs:
INNER JOIN (or JOIN): Returns records that have
matching values in both tables.
LEFT JOIN (or LEFT OUTER JOIN): Returns all records
from the left table and the matched records from the right
table.
RIGHT JOIN (or RIGHT OUTER JOIN): Returns all
records from the right table and the matched records from
the left table.

---

## Page 26

FULL JOIN (or FULL OUTER JOIN): Returns all records
when a match is in either the left or the right table.
Imagine two tables:
To combine these tables using an INNER JOIN based on the
AuthorID, you would use:
JOIN Operations: Combining Tables (LEFT JOIN/ LEFT OUTER
JOIN)
Returns all records from the left table and the matched records from
the right table. If there is no match, the result is NULL.

---

## Page 27

Using the LEFT JOIN:
JOIN Operations: Combining Tables (RIGHT JOIN / RIGHT
OUTER JOIN))
Returns all records from the right table and the matched records
from the left table. If there is no match, the result is NULL.

---

## Page 28

The left table is 'Authors' and the right is 'Books'.
JOIN Operations: Combining Tables (FULL JOIN / FULL OUTER
JOIN))
Returns all records when a match is in the left or the right table.

---

## Page 29

JOINS Table Aliasing:
In SQL, table aliasing is a technique that assigns a temporary name
to a table. This is particularly useful when working with joins,
especially when joining a table with itself or when joining tables with
long names. Table aliasing not only makes our SQL code more
readable but also ensures that there are no ambiguities when
referencing columns.

---

## Page 30

Image that we want to retrieve a list of employees and their
managers. Since the manager's information is also stored in the
Employees table, we need to join the table with itself. Here, table
aliasing becomes essential.
In this query, e1 and e2 are aliases for the Employees table. This
allows us to differentiate between the Employee and their manager.
COALESCE
The COALESCE function in SQL is a powerful tool that allows you to
return the first non-null value in a list of expressions. It is
beneficial when you want to provide a default value for columns that
might contain null values. Essentially, COALESCE scans through its

---

## Page 31

arguments in order and returns the first non-null value it encounters.
If all arguments are null, it returns null.
Imagine we want to retrieve a list of employees and their respective
managers. However, some employees might not have a manager
(as indicated by a NULL value in the manager_id column). We want
to display 'No Manager' instead of a null value in such cases.
In this query, the COALESCE function checks if e2.emp_name is
null and, if so, returns 'No Manager'.
GROUP BY: Aggregating Data

---

## Page 32

The GROUP BY statement is used in SQL to group rows with the
same values in specified columns into summary rows. It is often
used with aggregate functions to calculate each group of rows.
These aggregate functions can compute the sum, average, count,
etc., of columns for each distinct group.
Using GROUP BY, you can transform detailed data into a
summarised form, making it easier to analyse patterns and insights.
Common aggregating functions in SQL include:
COUNT(): Counts the number of rows in a group.
SUM(): Adds up the values in a numeric column for all
rows in a group.
AVG(): Calculates the average value of a numeric column
for all rows in a group.
MIN(): Returns the smallest value in a column for all rows
in a group.
MAX(): Returns the largest value in a column for all rows in
a group.
Imagine you have a table named 'Books' with columns 'AuthorID',
'Title', and 'YearPublished'.
To count the number of books by each Author, you would use: (Here
the as is just another method to rename the column, e.g., Title to
NumberofBooks)

---

## Page 33

HAVING: Filtering Aggregated Data
The HAVING clause is used with the GROUP BY clause to filter the
results based on a condition applied to the aggregated data. While
the WHERE clause filters individual rows before they are grouped,
the HAVING clause filters groups after aggregation. This makes the
HAVING clause essential when setting conditions on aggregated
data.
Imagine you have a library and want to identify authors who have
written multiple books. Instead of sifting through each book manually,
you can use the HAVING clause to filter out authors based on the
number of books they have written.
Using the Books table, let us find authors who have written more
than one book:

---

## Page 34

UNION
The UNION operator combines the result sets of two or more
SELECT statements. It removes duplicate rows from the combined
result set.
To retrieve a list of all unique book titles, both fiction and non-fiction,
you would:

---

## Page 35

UNION ALL
The UNION ALL operator is like UNION but does not remove
duplicate rows from the combined result set.
To retrieve a list of all book titles, both fiction and non-fiction,
including duplicates, you would use:

---

## Page 36

When to Use:
Preserving Duplicates: If you want to combine results
from multiple SELECT statements and retain all rows,
including duplicates, UNION ALL is the choice.
Performance: UNION ALL is faster than UNION because
it does not have to check for duplicates. If you are dealing
with large datasets and know there are no duplicates (or
duplicates do not matter), UNION ALL can be more
efficient.
Data Analysis and Reporting: In some scenarios, you
might want to analyse the full volume of data, including
repetitions. For instance, if you are analysing sales from
different regions and want to see the total number of sales,
even if some sales are recorded in multiple regions.
Functions and Subqueries
SQL functions are built-in operations that perform calculations on
data, such as finding a column's average, sum, or count.
Subqueries, on the other hand, are queries nested inside other
queries. They allow you to retrieve data used in the main query as a

---

## Page 37

condition to refine the results further.
Using the Books table above, use functions to find the average year
of publication:
Notice that since this is a singular metric, we do not need to use the
GROUP BY clause even though we are aggregating data.
Example for Subqueries:
To find books by the Author who wrote "SQL Basics":
Here, we can see that the Author who wrote the book "SQL Basics"
is "John Dow," which becomes our filtering criteria to return all books
by this Author.

---

## Page 38

However, this is just a simple example. In real-world examples,
subqueries could allow for more complex data retrieval based on the
results of another query. Let us delve into a more intricate example
to showcase the potential of subqueries.
Scenario
Imagine you want to find out which authors have total sales that rank
in the top 3 of all authors. For this, you have two tables: Books and
Sales.
To find authors whose total sales rank in the top 3:

---

## Page 39

We first join the Books and Sales tables on BookID.
We group the results by Author and calculate the total
sales for each Author using the SUM function.
The HAVING clause filters out authors based on their total
sales. The subquery within the HAVING clause retrieves
the third-highest total sales amount among all authors.
This ensures we only get authors whose sales are in the
top 3.
Finally, we order the results by TotalSales in descending
order to get the top-selling authors at the top.
Creating CTEs (Common Table Expressions)
A Common Table Expression (CTE) provides a way to define a
temporary result set that can be easily referenced. CTEs help break
down complex queries into simpler parts, making the SQL more
readable and maintainable. They are defined using the WITH
keyword.

---

## Page 40

Imagine you have a table, 'Employees', with columns EmployeeID,
EmployeeName, and ManagerID. If you want to retrieve a
hierarchical list of employees and their managers, you would use a
recursive CTE.
Here, we define the temporary table as RecursiveCTE, then write
our query to populate this temporary table inside it. After which, we
can query directly from it in the same query.

---

## Page 41

CTEs and subqueries make up a lot of modern-day SQL queries, but
it is essential to know the differences in when to use either:
When to Use: CTEs (Common Table Expressions)
Readability: A CTE can make your query more readable if
you have a complex query with multiple levels of
subqueries. CTEs allow you to name your temporary result
sets, making the main query easier to understand.
Reuse: If you need to reference the same subquery
multiple times in your main query, a CTE can be more
efficient if you define it once and then reference it
numerous times.
Recursive Queries: Think of CTEs as a tool that can
repeatedly ask a question until it gets all the answers,
especially when those answers are linked in a chain or
tree-like structure. Subqueries cannot do this repeated
asking on their own.
Modularity: CTEs can be stacked, meaning you can
define one CTE after another and use the result of one
CTE in the next. This can help in breaking down very
complex logic into modular parts.
When to Use: Subqueries
Simplicity: A subquery can be more straightforward and
intuitive for simple queries where you need to fetch a value
or a set of values to be used in the main query.
Inline Logic: If the logic of the subquery is closely tied to
the main query and does not need to be reused or
separated for clarity, an inline subquery might be more
appropriate.
Contained Logic: If you have a piece of logic that is better
kept "contained" within the main query (e.g., it is not going
to be reused, and it is not overly complex), a subquery can
be a good choice.
Performance: In some database systems, using a
subquery might be faster than a CTE, especially for simple

---

## Page 42

operations. However, this can vary based on the database
system, specific query, and data.
Window Functions
SQL Window Functions, often called "window functions," are a
subset of SQL functions that allow you to perform calculations
across a set of table rows related to the current row. Unlike
aggregate functions, which return a single value for a group of rows,
window functions return a single value for each row from the original
result set based on a defined window of rows.
The power of window functions lies in their ability to provide
advanced analysis and insights without collapsing or aggregating the
data. They operate within a "window" of rows defined by the OVER
clause, determining the range or set of rows used for calculations.
This window can be defined in various ways, such as ordering rows
by a particular column or grouping rows based on specific criteria.
Common use cases for window functions include:
Calculating running totals or averages.
Ranking data.
Finding the difference between current and previous row
values.
Calculating percentiles or cumulative distributions.
By using window functions, you can gain deeper insights into your
data and perform complex analyses without requiring multiple
subqueries or joining tables many times.
Calculating Running Totals
You have a table named Sales that contains monthly sales data for a
year. You want to calculate the running total for each month.

---

## Page 43

Window functions allow you to perform calculations across table
rows related to the current row. In this scenario, we use the SUM()
function as a window function to calculate the running total.
Ranking Sales Representatives
In the RepSales table, you have sales data for various sales
representatives. You want to rank them based on their sales
performance.

---

## Page 44

The RANK() window function assigns a unique rank to each distinct
row within a result set based on the values in one or more columns.
DENSE_RANK()
Like RANK(), the DENSE_RANK() function assigns a rank to each
row. However, it does not skip any rank if there is a tie.

---

## Page 45

Calculating the Difference from the Previous Month
Using the Sales table, you want to calculate the difference in sales
from the previous month.
LAG(SalesAmount, 1, 0) OVER (ORDER BY Month) is a
window function that fetches the SalesAmount from the
previous row (as defined by the ORDER BY Month
clause). If there's no last row (i.e., for the first month), it
defaults to 0.
SalesAmount - LAG(SalesAmount, 1, 0) OVER (ORDER
BY Month) computes the difference between the current
and previous months' sales.

---

## Page 46

Splitting Metrics into Quartiles
The NTILE function divides the result set into a specified number of
roughly equal parts. It is helpful for tasks like dividing a dataset into
quartiles, deciles, or any other "tile".
Imagine you have a list of students and their scores. You want to
divide them into four groups (quartiles) based on their scores.

---

## Page 48

Chapter 4: Common Real-World SQL Issues
(Working with Timestamps)
This book section will dive into common real-world SQL use cases
and serve as an example of effectively applying SQL techniques in
practical scenarios.
Dealing with Timestamp Data by Truncating Timestamp Data
Often, logs are stored in a database in a timestamp format, e.g.,
'2023-10-20 14:35:21.123' down to the millisecond. While this
precision is great for logging, it can be cumbersome for analysis. We
can simplify our data by truncating timestamps for more
straightforward aggregation and reporting.

---

## Page 49

You often must aggregate this data by day, week, month, or quarter.
Instead of dealing with detailed timestamps, you would want to
truncate them to a specific format, such as "YYYY-MM-DD".
To truncate the timestamp to a day:
Similarly, you can replace the 'day' portion with 'week', 'month' or
'quarter' to truncate the timestamp to the beginning of the period,
respectively.
Conversion of UNIX to a Readable Timestamp Data
Sometimes, timestamps are stored in UNIX format, which is a count
of seconds since January 1, 1970. You want to convert this to a
human-readable form.

---

## Page 50

UNIX timestamps are great for computers but hard for humans to
understand. Converting them to a standard date-time format makes
them easier to read and analyse.
Converting Time or Date Data to Respective Time Zone
Imagine you have a global e-commerce website. Customers from all
over the world place orders, but the timestamps are in UTC. For a
regional analysis, you want to convert these timestamps to the
respective local time zones to provide more accurate insights.

---

## Page 52

Chapter 5: Common Real-World SQL Issues
(Working with JSON Data)
In today's data-driven world, JSON (JavaScript Object Notation) has
become a popular format for data interchange. It is lightweight,
human-readable, and easy to parse.
Databases have evolved to support JSON data types and offer
functions to extract and manipulate this data. This chapter will
explore real-world scenarios where you might need to work with
JSON data in SQL.
Extracting Key-Value Pairs from JSON Data
JSON data are stored In Key-Value Pairs.
In this case, the Key would be "age", and the value would be 25, for
example.
To extract specific attributes (age, hobby, and city) from the JSON
data in the Details column for each user:

---

## Page 53

Querying Nested JSON Data
The following reference data shows that the JSON is nested within
another variable. For example, street is nested under the address
Key.
To extract the user's age and their nested address details (street and
zip code) from the JSON data in the Details column:

---

## Page 54

Filtering Rows Based on JSON Data
We can also include JSON clauses to filter rows on JSON data.
For example, to find all users from the UserProfiles table who have a
hobby of "reading".

---

## Page 55

Chapter 6: Common Real-World SQL Issues
(Cleaning String Data)
Data might not always be as clean as we would like it to be in the
real world. Some common issues might include extra whitespaces
found in data or inconsistent letter casing.
Removing Extra Spaces
A table named ProductList contains product names. However, some
product names have extra spaces at the beginning or end. As such,
this might affect the output if you are querying and somehow miss
the extra space in the product name.

---

## Page 56

To trim the extra spaces from the product names to ensure
consistency:
Converting Text to Proper Case
In the CustomerInfo table, the customer names are stored in
uppercase. You want to convert them to proper case (first letter
capitalised).

---

## Page 57

Extracting Domain from Email Addresses
You have a table named UserEmails that contains user email
addresses. You want to extract just the domain name from each
email.

---

## Page 58

Chapter 7: Common Real-World SQL Issues
(Working with Arrays)
Storing Multiple Values in a Single Column
Arrays in SQL allow you to store multiple values in a single column.
This can be particularly useful when you have a set of related values
that you want to associate with a single record, such as tags for a
blog post or phone numbers for a contact.

---

## Page 59

To retrieve blog posts tagged with "SQL" and "Advanced". The <@
operator checks if the array on the right is contained within the array
on the left.
Adding and Removing Elements from an Array
SQL provides functions to add or remove elements from an array.
This is useful when updating the values stored in an array column.
To add a new PhoneNumber to an existing entry:

---

## Page 60

Querying Specific Array Elements
You can query specific elements of an array using array indexing.
This is useful when retrieving or checking a particular value within an
array.
To retrieve the second item from the Items array for each order:
Expanding Arrays with UNNEST
The UNNEST function is used to transform arrays into a set of rows.
This is particularly useful when you have a column storing arrays
and want to perform operations on individual elements of those
arrays.

---

## Page 61

The code uses the UNNEST function to transform the Hobbies array
column into individual rows for each hobby. This allows for easier
querying and analysis of individual hobbies.
Aggregating Rows into Arrays with ARRAY_AGG
The ARRAY_AGG function is used to aggregate multiple rows into a
single array. This is particularly useful when you want to group data
and represent multiple related values as an array within a single row.

---

## Page 62

The code uses the ARRAY_AGG function to aggregate the
ProductName column into an array for each UserID. This provides a
concise representation of all products purchased by each user.
Extracting Common Values from Two Array Columns
When working with tables that have array columns, there might be
scenarios where you want to find the common elements between
two arrays. This can be achieved using array functions and
operators.
This approach identifies common elements between two array
columns, which can be helpful for various analytical purposes, such
as understanding user behaviour or preferences.

---

## Page 63

The code uses the UNNEST function to expand the LikedProducts
and PurchasedProducts arrays. The INTERSECT operator then
finds the common elements between the two arrays for each user.

---

## Page 64

Chapter 8: Common SQL Technical Interview
Questions
Lastly, before we wrap up this book, I would also love to include
some typical and real-world SQL questions that could be asked in
technical interviews:
Question: How would you retrieve the second highest salary from a
table named 'Employees'?

---

## Page 65

Strategy: Use a subquery to find the maximum salary, and then, in
the main query, find the maximum salary that is less than the value
from the subquery.
Question: How would you find the total number of orders placed by
each customer?
Strategy: Use the GROUP BY clause to group the results by
customer and the COUNT function to count the number of orders for
each customer.

---

## Page 66

Question: How would you find all customers who have not placed
any orders?
Strategy: Use a subquery to retrieve all customer IDs from the
'Orders' table and then find customers not on that list.
Question: How would you count the number of distinct products
ordered by each customer?
Strategy: Use the COUNT and DISTINCT functions to count unique
product IDs for each customer.

---

## Page 67

Question: Identify the top 3 products by sales amount per month
from the 'ProductSales' table.
Strategy: Use a subquery or a Common Table Expression (CTE) to
filter the results based on the rank.

---

## Page 68

Question: Retrieve a List of Employees and Their Managers
Strategy: We can perform a self-join on the Employee's table to
match each Employee with their manager.

---

## Page 69

Question: Retrieve a list of products and their respective categories.
Strategy: Join the Products table with the Categories table on the
category_id to match each product with its category.

---

## Page 70

Question: Identify Customers Without Orders
Strategy: Perform a left join between Customers and Orders tables
on customer_id and filter the results where order_id is NULL.

---

## Page 72

Chapter 9: Moving Forward
As we draw this book to a close, it is essential to recognise that
mastering SQL is an ongoing journey. The examples, guides, and
scenarios presented throughout these pages are a foundational
stepping stone designed to equip you with the fundamental skills and
knowledge to navigate the vast world of SQL. However, like any
other skill, true proficiency in SQL comes with consistent practice
and real-world application.
While this book provides a structured pathway to understanding
SQL, it is merely the beginning. The real challenge and reward come
from applying what you have learned in diverse and complex
scenarios, pushing the boundaries of your understanding, and
continuously seeking to improve.
For those eager to continue honing their SQL skills, numerous
platforms offer various SQL coding challenges, ranging from
beginner to expert levels. Platforms such as LeetCode and
HackerRank provide a vast array of SQL problems to solve and
allow you to engage with a community of like-minded individuals.
LeetCode Interface

---

## Page 73

HackRank Interface
Also, practice makes perfect, and in modern-day technical
interviews, online assessments often draw inspiration from questions
commonly found on these platforms. Familiarising yourself with
these platforms sharpens your skills and gives you a competitive
edge when facing real-world interview scenarios.
