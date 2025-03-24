# Pizza-sales-analysis-SQL
## Project Overview

**Project Title**: Pizza Sales Analysis  
**Level**: Beginner  
**Database**: `p1_retail_db`

This project is designed to demonstrate SQL skills and techniques typically used by data analysts to explore, clean, and analyze pizza sales data. The project involves setting up a pizza sales database, performing exploratory data analysis (EDA), and answering specific business questions through SQL queries. This project is ideal for those who are starting their journey in data analysis and want to build a solid foundation in SQL.

## Objectives

1. **Set up a retail sales database**: Create and populate a pizza sales database with the provided sales data.
2. **Data Cleaning**: Identify and remove any records with missing or null values.
3. **Exploratory Data Analysis (EDA)**: Perform basic exploratory data analysis to understand the dataset.
4. **Business Analysis**: Use SQL to answer specific business questions and derive insights from the sales data.

## Project Structure

### 1. Database Setup

- **Database Creation**: The project starts by creating a database named `orders`,`orders_details`.
- **Table Creation**: A table named `pizza_sales` is created to store the sales data. The table structure includes columns for order_id, order_data, order_time, order_deatils_id, pizza_id and quantity.

```sql
create database pizzahuts;

create table orders(
	order_id int not null,
    order_date date not null,
    order_time time not null,
    primary key(order_id)
);

create table orders_details(
	order_details_id int not null,
	order_id int not null,
    pizza_id text not null,
    quantity int not null,
    primary key(order_details_id)
);
```
