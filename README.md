# ecommerce-analysis
Analysis of synthetic e-commerce data to answer specific questions using Python and SQL.

## Objectives
This is a portfolio project aimed at exercising MySQL and Python for data analysis.
The main objective during this exercise is to answer some business-related questions described in the following tasks.

## Tasks

### Task 0
Set up a MySQL database named ecommerce_db with three tables:
- **customers**: containing the **name** and the **country** of the customer
- **products**: containing the **name** and the **category** of the product
- **sales**: holding **sales transactions** that identify the customer, the product, the quantity, the unit price, and the sales date from the beginnning of 2021 to the end of 2022

Remarks:
- Only one product is bought in a transaction.
- Data can be generated (synthetic).
- Before creating the database, it shall be checked, if a database with the same nem already exists. 

### Task 1
What is the total revenue for each product category in 2022?
### Task 2
What is the top-selling product for each month in 2022?
### Task 3
Identify the customers who are within the top 10% in terms of generating revenue in 2022.

## Solutions
### Task 0
I generated a small of batch of data for each table using ChatGPT, and saved them in .csv files respectively.
These can be found in the `data` folder.
```shell
|── data
    ├── CUSTOMERS.csv
    ├── PRODUCTS.csv
    └── SALES.csv

```
The database is set up by the `create_db()` function. It creates tha database with the three tables and fills the tables with data stored in the .csv files.
The very simple shcema can be senn in Figure 1.

<figure>
<img src="images/chicago_crime_download.png" width="100%" align="center"/></a>
<figcaption> Figure 1 - Database schema</figcaption>
</figure>

### Task 1

