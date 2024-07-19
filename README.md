### Project e-commerce

Sales data from the online store.
There are three data tables:
1. df_orders - Orders table 
2. df_customers - Table with unique user identifiers
3. df_item - Items included in orders

I will analyze completed purchases and answer the following questions:
1. How many users have made a purchase only once?
2. On average, how many orders per month are not delivered for various reasons? (Provide a breakdown by reasons)
3. For each item, determine which day of the week it is most frequently purchased.
4. How many purchases per week does each user make on average (per month)?
5. I will perform cohort analysis of users.
6. I will build RFM segmentation of users to qualitatively assess our audience.

Orders table df_orders
- order_id — unique order identifier (receipt number)
- customer_id — customer identifier per order
- order_status — order status
- order_purchase_timestamp — order creation time
- order_approved_at — order payment confirmation time
- order_delivered_carrier_date — time the order was handed over to the logistics service
- order_delivered_customer_date — order delivery time
- order_estimated_delivery_date — promised delivery date

Users table df_customers
- customer_id — customer identifier per order
- customer_unique_id — unique customer identifier (similar to a passport number)
- customer_zip_code_prefix — customer's postal code
- customer_city — customer's delivery city
- customer_state — customer's delivery state

Items table df_items
- order_id — unique order identifier (receipt number)
- order_item_id — item identifier within an order
- product_id — product ID (similar to a barcode)
- seller_id — product manufacturer ID
- shipping_limit_date — latest delivery date for the seller to hand over the order to the logistics partner
- price — price per item
- freight_value — freight weight
