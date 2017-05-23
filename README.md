![GitHub Logo](https://s3.ap-south-1.amazonaws.com/greyatom-social/GreyAtom-logo.png)

# SELF JOINS

The SQL SELF JOIN is used to join a table to itself as if the table were two tables; temporarily renaming at least one table in the SQL statement.

### Syntax

        SELECT a.column_name, b.column_name...
        FROM table1 a, table1 b
        WHERE a.common_field = b.common_field;

Here, the WHERE clause could be any given expression based on your requirement.

Now, let us join Customers table using SELF JOIN as follows −

        SELECT  a.CustomerID, b.CustomerName
           FROM Customers a, Customers b
           WHERE a.CustomerID = b.CustomerID;
