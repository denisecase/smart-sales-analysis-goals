# 3-SALES_PERFORMANCE_BY_STORE

## Overview
Analyze the total sales performance across different stores to identify trends and optimize resource allocation. 
This analysis can guide decisions related to store-specific marketing efforts, inventory distribution, or future store expansions.

## Required Data Columns
- StoreID: Identifier for the store where the transaction occurred.
- SaleAmount: Total revenue from each sale.

## Data Preparation Steps
- Ensure that each transaction is linked to the correct store using StoreID from the Sales table.

## Calculation Instructions
1. Group transactions by StoreID.
2. Sum SaleAmount for each store.
3. Optionally, calculate the percentage of total sales contributed by each store.

## Expected Outcome
A ranked list of stores based on total sales performance.

## Data-Driven Decision (DDDM)
KPI: Sales Revenue by Store.
- Action: Allocate resources such as inventory, staffing, or marketing based on the performance of each store. For lower-performing stores, consider targeted marketing efforts or operational adjustments to boost sales.

## Additional Notes
- We don't usually refer to stores just by their ID — instead, we typically use a name or a location. 
- RECOMMENDED: Create a Store Dimension Table if not already present to store additional store-specific attributes, such as:
  - StoreName: Name of the store.
  - City: City where the store is located.
  - State: State where the store is located.
  - Size: Physical size of the store.
  - LocationType: Type of location (urban, suburban, rural).

- REMINDER: Ensure referential integrity by verifying that each StoreID in the Sales table corresponds to a valid StoreID in the Store Dimension Table.

## Difficulty Level
3
