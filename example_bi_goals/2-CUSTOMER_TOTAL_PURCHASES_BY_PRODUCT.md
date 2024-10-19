# 2-CUSTOMER_TOTAL_PURCHASES_BY_PRODUCT

## Overview
Determine how much each customer spends on individual products. 
This analysis helps understand customer preferences and product performance across the customer base.

## Required Data Columns
- CustomerID: Unique identifier for each customer.
- ProductID: Unique identifier for each product.
- SaleAmount: Total revenue from each sale.

## Data Preparation Steps
- Ensure each transaction links the CustomerID with the purchased ProductID.

## Calculation Instructions
1. Group the data by both CustomerID and ProductID.
2. Sum SaleAmount for each customer-product combination to determine total spending on each product by each customer.

## Expected Outcome
A report showing the total amount spent by each customer on each product.

## Data-Driven Decision (DDDM)
KPI: Customer Spending by Product.
- Action: Identify customer preferences for certain products and tailor marketing efforts, product recommendations, or personalized offers based on customer purchase behavior.

## Difficulty Level
2
