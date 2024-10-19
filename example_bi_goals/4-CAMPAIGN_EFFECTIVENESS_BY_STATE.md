# 4-CAMPAIGN_EFFECTIVENESS_BY_STATE

## Overview
Evaluate the effectiveness of marketing campaigns by state. 
This analysis helps determine which marketing campaigns perform better in specific regions, guiding future marketing strategies and budget allocation. 

It may involve a Store Dimension Table which provides the State information for the sale. 
The Store Dimension Table would contain information about each store, such as city, state, and zipcode, which can be joined to the Sales data to analyze campaign performance across different regions.

## Required Tables and Columns

### Sales Table
- TransactionID: Unique identifier for each sale.
- CampaignID: Identifier for the marketing campaign.
- StoreID: Identifier for the store where the transaction occurred.
- SaleAmount: Total revenue from each sale.

### Store Dimension Table (Newly Created)
- StoreID: Unique identifier for each store (links to the Sales table).
- StoreName: Name of the store.
- City: City where the store is located.
- State: State where the store is located (used for analysis).
- ZipCode: Store's postal code (optional for deeper analysis).

### Campaign Dimension Table (Optional)
- CampaignID: Unique identifier for each campaign (links to the Sales table).
- CampaignName: Name of the campaign.
- StartDate: Start date of the campaign.
- EndDate: End date of the campaign.

## Data Preparation Steps
1. Create the Store Dimension Table: Build a Store Dimension Table that contains detailed geographic information, including the state where each store is located. Ensure each sale links to the correct store through the StoreID.
   
2. Join Tables: Join the Sales table with the Store Dimension Table using StoreID to obtain the State data for each sale.

3. Link to Campaigns: Ensure that each sale is associated with a marketing campaign by linking the Sales table to the Campaign Dimension Table via CampaignID.

## Calculation Instructions
1. Group transactions by State and CampaignID.
2. Sum SaleAmount for each combination of State and CampaignID.
3. Compare sales performance of different campaigns across states to identify regional preferences.

## Expected Outcome
A report showing the effectiveness of different marketing campaigns by state, highlighting which campaigns generate the most revenue in specific regions.

## Data-Driven Decision (DDDM)
KPI: Campaign Effectiveness by State.
- Action: Based on the results, adjust marketing efforts. Focus on the states where specific campaigns have proven to be effective, and for underperforming regions, consider modifying campaign strategies or reallocating marketing budgets.

## Additional Notes
- Create a Campaign Dimension Table to track additional attributes about each campaign, such as type, duration, and cost.
- IMPORTANT: Ensure all state-related data is accessed through the Store Dimension Table and not directly from the Sales table. This ensures referential integrity and avoids redundancy.

## Referential Integrity Reminder
Always ensure that each StoreID in the Sales table has a corresponding entry in the Store Dimension Table. This helps avoid errors in geographic analysis and ensures accurate results.

## Difficulty Level
4
