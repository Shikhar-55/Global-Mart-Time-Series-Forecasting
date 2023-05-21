# Global-Mart-Time-Series-Forecasting


Global Mart is an online supergiant store that operates worldwide, catering to consumer, corporate, and home office segments. As a sales manager for Global Mart, your task is to forecast the sales of products for the next 6 months. This forecast will enable you to plan inventory and business processes effectively.

### Dataset
To access the necessary data for sales forecasting, download the Global Superstore Dataset. The dataset includes the following attributes:

Order-Date: The date on which the order was placed.

Segment: The segment to which the product belongs.

Market: The market to which the customer belongs.

Sales: Total sales value of the transaction.

Profit: Profit made on the transaction.

The dataset provides information on 21 unique market segments, categorized by geographical market regions and customer segments.

### Finding the Most Profitable Market Segment
To identify the most consistently profitable market segment, we will use the "Coefficient of Variation (CoV)" measure. The CoV is the ratio of the standard deviation to the mean for a given dataset. In this case, we will calculate the CoV for each of the 21 market segments based on their profitability.

By normalizing the standard deviation with the mean using the CoV, we can compare the variation in profits across different market segments effectively. The market segment with the least variation in profits will be considered the most consistently profitable.

### Data Understanding and Preparation
To perform data preparation and analysis, follow these steps:

Combine the 7 geographical markets for each of the 3 segments: Combine the market data to obtain the 21 unique market segments.

Structure the dataset: Reorganize the dataset to include the Order-Date, Sales, and Profit for each market segment (e.g., APAC-Consumer, APAC-Home Office, etc.).

Convert Order-Date: Convert the Order-Date into a month-year format for monthly aggregation of transactions.

Perform a train-test split: Split the data into a training set and a test set. Use the first 42 months as the training data and the last 6 months as the test data.

Calculate the CoV: Calculate the CoV on the profit for each of the 21 market segments using the training data.

Compare the CoV values: Compare the CoV values to determine the most profitable market segment.

Sales Forecasting for the Most Profitable Market Segment
Once you have identified the most profitable market segment, the next step is to forecast the sales specifically for that segment. This will allow you to focus on a reliable market region for accurate sales predictions.
