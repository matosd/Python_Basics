# Python_Repository

This repository contains a series of Jupyter notebooks for various data analytics projects.

## 1. Instacart Grocery Basket Analysis (June 2024)

<img width="182" alt="image" src="https://github.com/matosd/Python_Repository/assets/26867481/a69ba6a8-cc29-4a8c-926c-42ca7bbe02c1">


### Introduction
Instacart is an online grocery store. The purpose of this project was to undertake an exploratory analysis to help uncovering more information about their sales patterns, including variety of customers and purchasing behaviours, to help create a targeted marketing strategy for the company.

### Data Sources
Instacart Market Basket Analysis: https://www.kaggle.com/datasets/psparks/instacart-market-basket-analysis

### Datasets
*See also Data Dictionary*

* Orders
* Orders_products_prior
* Products
* Departments
* Customers

### Tools
* pandas
* numpy
* matplotlib
* seaborn
* scipy

### Folders
* 03 Scripts
* 04 Analysis
* 05 Sent to Client

### Data Dictionary

#### ORDERS dataset
*Data associated with each order*

* order_id: order identifier
* user_id: customer identifier
* order_number: the order sequence number for this user
* order_day_of_week: the day of the week the order was placed, where:
	* 0 = Saturday
	* 1 = Sunday
	* 2 = Monday
  * 3 = Tuesday
	* 4 = Wednesday
	* 5 = Thursday
	* 6 = Friday
* order_hour_of_day: the hour of the day the order was placed on
* days_since_prior: days since the last order, capped at 30 (with NAs for order_number = 1)

#### ORDERS_PRODUCTS_PRIOR dataset
*Further data associated with each order*

* order_id: order identifier
* product_id: product identifier
* add_to_cart_order: order of products as they are ordered by the customer
* reordered: whether a product has been previously ordered

#### PRODUCTS dataset
*Data associated with the products sold by Instacart*

* product_id: product identifier
* product_name: name of the product
* department_id: foreign key
* aisle_id: foreign key (eventually dropped)

#### DEPARTMENTS dataset
*List of departments*

department_id: department identifier
department: the name of the department

#### CUSTOMERS dataset
*This dataset was fabricated, for learning purposes*

* user_id: customer identifier
* name: customer’s first name (not included in the final analysis)
* surname: customer’s last name (not included in the final analysis)
* gender: customer’s gender
* state: customer’s location
* age: customer’s age
* family_status: customer’s marital status
* n_dependants: number of customer’s dependants
* income: customer’s yearly income
