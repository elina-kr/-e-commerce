# E-commerce 
## Overview
This project focuses on analyzing sales data from an online store to gain insights into customer behavior, order fulfillment, and item popularity. The data consists of three main tables: `df_orders` (orders), `df_customers` (customers), and `df_item` (items in orders). The analysis aims to address specific business questions regarding customer purchase patterns, order delivery issues, and item popularity.

## Goals
The primary objectives of this project are:
1. Determine the number of users who made a single purchase.
2. Analyze the average number of undelivered orders per month, categorized by reasons for non-delivery.
3. Identify the most common day of the week for purchases of each item.
4. Calculate the average number of purchases per week per user.
5. Perform cohort analysis to track user retention over time.
6. Conduct RFM (Recency, Frequency, Monetary) segmentation to evaluate customer value and behavior.

## Data Description
The project utilizes the following datasets:
- **`olist_customers_datase.csv`**: Contains unique user identifiers and location information.
  - `customer_id`: Order-specific user ID.
  - `customer_unique_id`: Unique user identifier.
  - `customer_zip_code_prefix`: User's postal code.
  - `customer_city`: User's city.
  - `customer_state`: User's state.

- **`olist_orders_dataset.csv`**: Contains information about each order.
  - `order_id`: Unique order identifier.
  - `customer_id`: Order-specific user ID.
  - `order_status`: Status of the order.
  - `order_purchase_timestamp`: Order creation time.
  - `order_approved_at`: Payment approval time.
  - `order_delivered_carrier_date`: Time when the order was handed over to the logistics service.
  - `order_delivered_customer_date`: Order delivery time.
  - `order_estimated_delivery_date`: Estimated delivery date.

- **`olist_order_items_dataset.csv`**: Details about items included in orders.
  - `order_id`: Unique order identifier.
  - `order_item_id`: Identifier for the item within an order.
  - `product_id`: Product identifier.
  - `seller_id`: Product manufacturer identifier.
  - `shipping_limit_date`: Latest date for the seller to hand over the item to logistics.
  - `price`: Item price.
  - `freight_value`: Shipping weight.

## Metrics for Evaluation
The following metrics are used to evaluate the results:
1. **User Purchase Frequency**: Number of users with only one purchase.
2. **Average Monthly Undelivered Orders**: Breakdown by reasons such as non-payment, delays in handover to logistics, system errors, logistics failure, and item unavailability.
3. **Day of the Week for Item Purchases**: Frequency of item purchases on specific days.
4. **Weekly Purchase Frequency per User**: Median of average weekly purchases per user.
5. **Cohort Retention Rate**: User retention and activity over time.
6. **RFM Segmentation Metrics**: Recency, Frequency, and Monetary value of purchases.


## Results
1. **Single Purchase Users**: 92,621 users made only one purchase.
2. **Undelivered Orders**: On average, 5.92 orders per month were not delivered due to non-payment, 49 due to delays in handover to logistics, 27 due to system errors, 48.5 due to logistics failures, and 27.36 due to item unavailability.
3. **Item Purchase Day**: Identified the most common day of the week for each item, with examples including Wednesday, Monday, and Thursday as frequent purchase days.
4. **Weekly Purchase Frequency**: The median value of average purchases per week per user was 0.23.
5. **Cohort Analysis**: The analysis revealed a significant number of new customers, with a large proportion being struggling customers (few purchases, low spending).
6. **RFM Segmentation**: Highlighted a significant number of new and struggling customers, indicating potential areas for targeted marketing efforts.

## Conclusion
The analysis provided valuable insights into customer behavior and order management. Identifying users with only one purchase and analyzing undelivered orders highlighted areas for improving customer retention and logistics processes. The cohort analysis and RFM segmentation offered a deeper understanding of customer segments, helping to inform future marketing and operational strategies.

## Key Skills
- Data Cleaning and Preprocessing
- Exploratory Data Analysis (EDA)
- Cohort Analysis
- RFM Segmentation
- Statistical Analysis
- Python (Pandas, NumPy, Matplotlib)
- SQL (for data extraction and manipulation)


## Contact
For any questions or additional information, please contact me at elina8kr@gmail.com. My LinkedIn: https://www.linkedin.com/in/elina-krs
