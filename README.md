# E-commerce 
## Overview
This project analyzes sales data from a UK-based online retailer that primarily sells unique all-occasion gifts. The dataset covers transactions from December 2010 to December 2011 across multiple countries.

The analysis explores customer purchases, product returns, profitability, and product categorization to generate actionable insights for inventory management and business strategy.

## Goals
The primary objectives of this project are:
1. Identify which products have been returned the most.
2. Analyze weekly, monthly, and quarterly profits from UK customers.
3. Test whether order sizes from countries outside the UK are significantly larger than those from UK customers.
4. Group the products into meaningful categories using clustering, based on price and sales volume, to assist with inventory management.

## Data Description
The dataset (`online_retail.csv`) contains the following fields:
- `InvoiceNo`: Unique 6-digit identifier for each transaction.
- `StockCode`: Unique 5-digit identifier for each product.
- `Description`: Name of the product.
- `Quantity`: Number of items per transaction (negative values indicate returns).
- `InvoiceDate`: Timestamp of the transaction.
- `UnitPrice`: Price per item in GBP.
- `CustomerID`: Unique 5-digit identifier for each customer.
- `Country`: Country of the customer.

## Metrics for Evaluation
The following metrics are used to evaluate the results:
1. **Most Returned Products**: Frequency of returns by product and return rate (proportion of returned items relative to total sold).
2. **Profitability Analysis**: Weekly, monthly, and quarterly revenue from UK customers.
3. **Order Size Comparison**: Statistical tests (t-test, Mann-Whitney U) and effect size (Cohen’s d) to determine differences in order sizes between UK and international customers.
4. **Product Segmentation**: K-means clustering of products based on quantity sold and average price to create meaningful product categories.

## Results
1. **Most Returned Products**: Top return-risk products are:
  - PAPER CRAFT, LITTLE BIRDIE – 80,995 units, 100% return rate
  - MEDIUM CERAMIC TOP STORAGE JAR – 74,494 units, 95.5% return rate
  - ROTATING SILVER ANGELS T-LIGHT HLDR – 9,376 units, 98.9% return rate
These items fail frequently and in high volume, suggesting priority for review.
2. **Revenue from UK Customers**:
  - Weekly: Sales are consistent, with a slight upward trend in later weeks.
  - Monthly: Recent months show stronger performance, indicating increased revenue.
  - Quarterly: Overall growth trend confirms steady sales with gradual increase.
3. **Order Size Comparison**: Non-UK customers place significantly larger orders than UK customers, with a meaningful difference.
4. **Product Segmentation**: Products were grouped into four segments, highlighting high-value items and lower-impact items. This segmentation helps guide marketing, stock, and strategic focus.

## Conclusion
The analysis provided actionable insights into product performance, customer behavior, and revenue trends. Identifying the most returned products highlighted critical return risks, while the revenue analysis from UK customers revealed stable and growing sales over time. Comparing order sizes showed that non-UK customers place significantly larger orders, informing potential pricing and marketing strategies. Finally, product segmentation clarified which items contribute most to revenue, supporting targeted marketing, stock management, and strategic planning. Overall, these findings help the business prioritize actions, optimize operations, and make data-driven decisions.

## Key Skills
- Data Cleaning & Preprocessing
- Exploratory Data Analysis (EDA)
- Time Series Aggregation (weekly, monthly, quarterly trends)
- Statistical Hypothesis Testing (t-test, Mann-Whitney U, Cohen’s d)
- K-Means Clustering
- Python (Pandas, NumPy, Matplotlib, Seaborn, SciPy, Scikit-learn)
