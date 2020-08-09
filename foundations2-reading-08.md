# SQL Bolt
https://sqlbolt.com/

* SQL is a relational database
    * A relational database represents a collection of related (two-dimensional) tables. Each of the tables are similar to an Excel spreadsheet, with a fixed number of named columns (the attributes or properties of the table) and any number of rows of data.

* to retrieve data from a SQL database, we write SELECT statements (or *queries*)
    * a query declares the data we are looking for, where to find it in the db and how to transform it, if we want it transformed

* syntax:
    ```SELECT whatever FROM whatevertable;```

* can also add WHERE clauses to queries in order to filter results
    ```js
    SELECT column, another_column, …
    FROM mytable
    WHERE condition
    AND/OR another_condition
    AND/OR …;
    ```
* **DISTINCT** allows you to filter out duplicate rows

* **ORDER BY** returns results in alpha-neumeric order either ascending or descending

* a table is called a schema and you can also add more data to it
    * done using **INSERT**

# W3 Schools SQL Practice
https://www.w3schools.com/sql/trysql.asp?filename=trysql_select_all