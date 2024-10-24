# Customer-Segmentation-Analysis

## Overview
This project aims to create customer segments using Power BI, helping businesses personalities understand their customer base better by analyzing purchasing behavior, demographics, and preferences. The segmentation is based on customer, transaction, and product data, allowing businesses to optimize marketing, sales, and customer service strategies across different regions.

## Datasets Taken
1. **customers.csv**: Contains details like customer age, gender, location, total spend, loyalty points, preferred payment method.
2. **transactions.csv**: Includes transaction history, purchase frequency, total spend, shipping addresses, delivery address.
3. **products.csv**: Contains product category information and purchase details.
4. **regions.csv**: Contains sales details across different regions.

## Customer Segments creation

### Data Cleaning process
#### 1. Import Datasets
- Use the "Get Data" feature in Power BI to load the required datasets (customers, transactions, products).
- In **Power Query Editor**, clean the data by:
  - Removing duplicates.
  - Handling missing values.
  - Ensuring the correct data types for all columns.

#### 2. Create Relationships
- Establish relationships between the datasets:
  - **Customer Dataset** and **Transaction Dataset**: Link via the `CustomerID` column.
  - If using a **Product Dataset**, link it to the **Transaction Dataset** via the `ProductID` column.

#### 3. Create Derived Columns
- **RFM Analysis**: Create new columns for:
  - **Recency**: Calculate the number of days since each customer’s last purchase.
  - **Frequency**: Count the total number of transactions per customer.
  - **Monetary Value**: Sum up the total amount spent by each customer.

- **Demographic Segmentation**:
  - **Age Groups**: Segment customers into predefined groups (e.g., 18-25, 26-35, etc.).
  - **Loyalty Tiers**: Categorize customers into low, medium, or high loyalty tiers based on loyalty points.
  - **Payment Methods**: Segment customers by their preferred payment method (e.g., PayPal, credit card).

## Conclusion
The datasets have been successfully cleaned and standardized. Each dataset now contains consistent, error-free, and well-structured data that can be used for analysis and reporting in Power BI.
