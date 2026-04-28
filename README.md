# Online Shopping Database (SQL)

This project is a beginner-to-intermediate level **E-commerce Database System** built using SQL.
It demonstrates how a real-world shopping system manages customers, products, and orders using relational database concepts.

## Features

* Customer management system
* Product management system
* Order processing system
* Use of **Primary Key** and **Foreign Key**
* Data retrieval using **INNER JOIN**
* Data analysis using **COUNT, SUM, AVG, GROUP BY**

## Database Structure

###  Customer Table

* `ID` (Primary Key)
* `NAME`

###  Products Table

* `PRODUCT_ID` (Primary Key)
* `NAME`
* `PRICE`

### Orders Table

* `ORDER_ID` (Primary Key)
* `CUSTOMER_ID` (Foreign Key)
* `PRODUCT_ID` (Foreign Key)
* `AMOUNT`

## Relationships

* One customer can place multiple orders
* One product can be ordered multiple times
* Tables are connected using **Foreign Keys**

##  Sample Query

```sql
SELECT CUSTOMER.NAME, PRODUCTS.NAME AS PRODUCT, ORDERS.AMOUNT
FROM ORDERS
INNER JOIN CUSTOMER ON CUSTOMER.ID = ORDERS.CUSTOMER_ID
INNER JOIN PRODUCTS ON PRODUCTS.PRODUCT_ID = ORDERS.PRODUCT_ID;
```


## Advanced Queries

* Total spending per customer using `SUM()` and `GROUP BY`
* Most sold product using `COUNT()`
* Filtering high-value customers using `HAVING`


## Technologies Used

* SQL (MySQL)


## How to Run

1. Create the database
2. Run the `shopping_db.sql` file
3. Execute queries to view results

##  Future Improvements

* Add Cart System
* Add Quantity and Order Date
* Connect with Java (JDBC)
* Build GUI-based shopping system
