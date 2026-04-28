#  Online Shopping Database (SQL)

This project is a beginner-friendly **E-commerce Database System** built using SQL.
It demonstrates how a real-world shopping system manages customers and orders using relational database concepts.

---

##  Features

* Create and manage customers
* Store and manage orders
* Use of **Primary Key** and **Foreign Key**
* Data retrieval using **JOIN**
* Basic analysis using **COUNT, SUM, AVG**

---

## Database Structure

### Customer Table

* `ID` (Primary Key)
* `NAME`

###  Orders Table

* `ORDER_ID` (Primary Key)
* `CUSTOMER_ID` (Foreign Key)
* `AMOUNT`

---

##  Relationships

* One customer can place multiple orders
* Tables are connected using Foreign Key

---

##  Sample Query

```sql
SELECT CUSTOMER.NAME, ORDERS.AMOUNT
FROM CUSTOMER
INNER JOIN ORDERS
ON CUSTOMER.ID = ORDERS.CUSTOMER_ID;
```

---

##  Technologies Used

* SQL (MySQL)

---

## How to Run

1. Create the database
2. Run the SQL file
3. Execute queries to see results

---

##  Future Improvements

* Add Products Table
* Add Cart System
* Connect with Java (JDBC)
