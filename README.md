# E-Commerce-Analysis

Problem statement: Understanding purchasing patterns is crucial for predicting behavior, improving retention, reducing churn, and maximizing customer lifetime value. A structured approach is needed to identify high-value customers, detect trends, and optimize targeted marketing strategies.

Objective: Utilize the RFM (Recency, Frequency, Monetary) framework to segment e-commerce customers. Analyse purchasing patterns to identify high-value customers and at-risk segments. Create targeted marketing strategies to improve customer retention and satisfaction.

DATASET OVERVIEW:
InvoiceNo: Contains the unique transaction ID
StockCode: Unique product identifier code
Description: Description of the product
Quantity: Number of items purchased
InvoiceDate: Timestamp of purchase
Unit Price: Price per unit of product
CustomerID: Unique customer identifier code
Country: Country in which the customer resides

Key Metrics: Total Sales (Quantity*Unit Sales), Total Volume, and Order Count. 
 
Data CLeaning: 
1. Percentage of missing values in CustomerID is 24.93%. Since the analysis revolves around investigating the customers and clustering them into categories, the missing values of customerid were removed. 
2. The number of duplicate rows in dataset is 5525. These rows where removed from the dataset.
3. Removed orders having negative values in quantity.
4. There are certain StockCode which don’t belong to any product. All the rows containing those stockcode were removed.

Insights from data after cleaning:
1. 26% of customers make 80% of the sales.
2. 21% of product make 80% of the sales.

Based on RFM Score Analysis, we have 4 customer segments: 
1. High Value Customers
2. Loyal Customers
3. At-Risk Customers
4. Dormant Customers

Recommendations:
1. High Value Customers
Behaviour: Low Recency (recent purchases), High Frequency, High Monetary Value.
Strategy: Priority loyalty rewards, Offer premium upgrades, and Encourage referrals or ambassador programs
2. Loyal Customers
Behaviour: Average Recency (but consistent over time), Moderately High Frequency, High Monetary Value.
Strategy: Introduce VIP loyalty tiers, Encourage subscription models, and Send reactivation nudges if recency drops.
3. At-Risk Customers
Behaviour: Low Recency, Moderately High Frequency, Moderately High Monetary Value.
Strategy: Launch win-back campaigns, Offer limited-time bundles or loyalty point top-ups, Monitor churn indicators closely.
4. Dormant Customers
Behaviour: Low Recency, Low Frequency, Low Monetary Value.
Strategy: Run re-engagement campaigns, Target with low-barrier offers, Move to low-cost email nurture campaigns.
