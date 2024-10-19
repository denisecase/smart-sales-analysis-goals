# CUSTOMER_AVERAGE_TRANSACTION_SIZE

## Overview
Calculate the average transaction size for each customer. 
Understanding average transaction sizes can help inform upselling strategies or customer segmentation.

## Required Data Columns
- CustomerID: Unique identifier for each customer.
- SaleAmount: The total value of each transaction.

## Data Preparation Steps
- Ensure each customer’s transactions are recorded accurately.

## Calculation Instructions
1. Group transactions by CustomerID.
2. Sum SaleAmount for each customer.
3. Divide the total sales by the number of transactions to calculate the average transaction size per customer.

## Expected Outcome
A list of customers and their respective average transaction sizes.

## Data-Driven Decision (DDDM)
KPI: Average Transaction Value (Total sales per transaction).
- Action: Focus upselling or promotional efforts on customers with lower transaction sizes, while offering personalized rewards to those with higher transaction sizes to encourage repeat business.

## Difficulty Level
1
