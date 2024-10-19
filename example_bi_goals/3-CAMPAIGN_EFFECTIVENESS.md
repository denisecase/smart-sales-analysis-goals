# 3-CAMPAIGN_EFFECTIVENESS

## Overview
Evaluate the effectiveness of marketing campaigns. 
This analysis helps determine which marketing campaigns generate the most revenue overall. 
To get a name for the campaign to go on the results, sample data for campaigns will be needed (e.g., campaign_data.csv or similar). Create a a record for every CampaignID in the sales_data.csv data and a Campaign Dimension Table to link sales data to specific marketing campaigns.

## Required Tables and Columns

### Sales Table
- TransactionID: Unique identifier for each sale.
- CampaignID: Identifier for the marketing campaign.
- SaleAmount: Total revenue from each sale.

### Campaign Dimension Table (Newly Created)
- CampaignID: Unique identifier for each campaign (links to the Sales table).
- CampaignName: Name of the campaign.
- StartDate: Start date of the campaign.
- EndDate: End date of the campaign.

## Data Preparation Steps
1. Create the Campaign Dimension Table: Build a Campaign Dimension Table that includes details like the campaign's name and duration (optional: start date and end date).
   
2. Link Campaigns to Sales: Join the Sales table with the Campaign Dimension Table using CampaignID to enrich the data with campaign names.

## Calculation Instructions
1. Group transactions by CampaignID.
2. Sum SaleAmount for each CampaignID.
3. Compare total sales across different campaigns.

## Expected Outcome
A report showing the total sales for each marketing campaign, showing which campaigns generate the most revenue.

## Data-Driven Decision (DDDM)
KPI: Total Sales per Campaign.
- Action: Focus marketing resources on the most effective campaigns. For underperforming campaigns, reassess the messaging or timing to improve future results.

## Additional Notes
- Make sure to create the Campaign Dimension Table to store campaign names and details.
- Expand the Campaign Dimension Table with additional attributes like campaign type or target audience in future analyses.

## Difficulty Level
3
