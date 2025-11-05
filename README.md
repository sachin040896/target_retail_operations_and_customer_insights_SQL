# target_retail_operations_and_customer_insights_SQL

## Company Description: <br>
1. Target is a well-established global brand and one of the leading retailers in the United States. It positions itself as a preferred shopping destination by delivering exceptional value, innovation, inspiration, and a customer experience unmatched by competitors. <br>
2. This case study examines Target’s operations in Brazil, analysing data from nearly 100,000 orders placed between September 2016 and August 2018. The dataset provides detailed insights into multiple aspects such as order status, pricing, payments, freight performance, customer locations, product details, and customer feedback. <br>
3. Through an in-depth exploration of this dataset, meaningful insights can be drawn about Target’s business performance in Brazil. These findings can help uncover patterns in order management, pricing models, payment and shipping efficiency, customer demographics, product trends, and levels of customer satisfaction. <br>

## Dataset Description: <br>
1. The customers table contain following features: <br>
i. customer_id - ID of the consumer who made the purchase <br>
ii. customer_unique_id - Unique ID of the customer <br>
iii. customer_zip_code_prefix - Zip code of consumers location <br>
iv. customer_city - Name of the city from where order is made <br>
v. customer_state - State code from where order is made <br>
2. The sellers table contains following features:
i. seller_id - Unique ID of seller registered <br>
ii. seller_zip_code_prefix - Zip code of the seller’s location <br>
iii. seller_city - Name of the city of seller <br>
iv. seller_state - State code <br>
3. The order_items table contains the following features: <br>
i. order_id - A unique ID of order made by the consumers <br>
ii. order_item_id - A Unique ID given to each item ordered in the order <br>
iii. product_id - A Unique ID given to each product available on the site <br>
iv. seller_id - Unique ID of the seller registered in Target <br>
v. shipping_limit_date - The date before which the ordered product must be shipped <br>
vi. price - Actual price of the product ordered <br>
vii. freight_value - Price rate at which a product is delivered from one point to another <br>
4. The geolocations table contains the following features: <br>
i. geolocation_zip_code_prefix - First 5 digits of Zip Code <br>
ii. geolocation_lat – Latitude <br>
iii. geolocation_lng – Longitude <br>
iv. geolocation_city – City <br>
v. geolocation_state – State <br>
5. The payment table contains the following features: <br>
i. order_id - A Unique ID of order made by consumers <br>
ii. payment_sequential - Sequences of the payments made in case of EMI <br>
iii. payment_type - Mode of payment used <br>
iv. payment_installments - Number of installments in case of EMI <br>purchase <br>
v. payment_value - Total amount made for the purchase order <br>
6. The orders table contains the following features: <br>
i. order_id - A Unique ID of order made by the consumers <br>
ii. customer_id - ID of the consumer who made the purchase <br>
iii. order_status - Status of the order made i.e., delivered, shipped etc <br>
iv. order_purchase_timestamp - Time stamp of the purchase <br>
v. order_delivered_carrier_date - Delivery date at which carrier made the delivery <br>
vi. ordered_delivered_customer_date - Date at which customer got the product <br>
vii. order_estimated_delivery_date - Estimated delivery date of the products <br>
7. The review table contains the following features: <br>
i. review_id - ID of review given on the product ordered by the order id <br>
ii. order-id - A Unique ID of order made by consumers <br>
iii. review_score - Review score given by customer for each order on a scale of 1-5 <br>
iv. review_comment_title - Title of the review <br>
v. review_comment_message - Review comments posted by the consumer for each order <br>
vi. review_creation_date - Timestamp of the review when it is created <br>
vii. review_answer_timestamp - Timestamp of the review answered <br>
8. The products table contains the following columns: <br>
i. product_id - A Unique identifier for the proposed project <br>
ii. product_category_name - Name of the product category <br>
iii. product_name_length - Length of the string which specifies the name given to the products ordered <br>
iv. product_description_length - Length of the description written for each product ordered on the site <br>
v. product_photos_qty - Number of photos of each product ordered available on the shopping portal <br>
vi. product_weight_g - Weight of the products ordered in grams <br>
vii. product_length_cm - Length of the products ordered in centimeters <br>
viii. product_height_cm - Height of the products ordered in centimeters <br>
ix. product_width_cm - Width of the product ordered in centimeters <br>
The dataset is relational and consists of 8 core tables that capture the end-to-end e-commerce process, from customer identity to product delivery and review. The tables can be linked through a set of key identifiers, forming a classic star/snowflake-like schema where the orders table acts as a central fact table connected to various dimension tables. <br>

## Recommendations: <br>

1. Seasonal Demand & Sales Strategy <br>
i. Capitalize on Q2–Q3 Demand Peaks (March–August): <br>
Increase marketing campaigns, discounts, and inventory levels during these months to maximize revenue when customer demand is at its highest. <br>
ii. Address the September Slump: <br>
Introduce targeted loyalty campaigns, back-to-school promotions, or limited-time discounts to counter the significant drop in September orders. <br>
iii. Holiday Season Readiness: <br>
Strengthen operations in November (festive season), ensuring optimized logistics and promotional offers to fully leverage shopping spikes. <br>

2. Regional Growth & Market Expansion <br>
i. Focus on Strong Markets (SP, RJ, MG): <br>
These states generate the highest customer volume and revenue. Target should invest in faster delivery guarantees, premium product offerings, and exclusive membership benefits here. <br>
ii. Develop Weaker Markets (North & Northeast states): <br>
Enhance brand visibility through localized advertising, influencer marketing, and partnerships with regional delivery providers to reduce freight costs and improve accessibility. <br>
iii. Balanced Resource Allocation: <br>
Use state-level demand data to guide inventory placement, warehouse expansion, and regional staffing decisions. <br>

3. Delivery & Logistics Optimization <br>
i. Improve Slow-Delivery States (SC, MG, DF, PR, SP): <br>
a. Establish micro-warehousing hubs closer to customers. <br>
b. Collaborate with 3rd-party logistics providers for last-mile delivery. <br>
c. Implement predictive stocking models based on historical demand. <br>
ii. Leverage Best Practices from High-Performance States (AM, AP, RR, AC, RO): <br>
Study logistics models in these regions (fast delivery times, ahead-of-estimate performance) and replicate successful strategies elsewhere. <br>
iii. Technology Adoption: <br>
Integrate real-time tracking systems and AI-powered delivery time predictions to reduce delays and improve customer trust. <br>

4. Payments & Financial Strategy <br>
i. Streamline Single-Installment Payments: <br>
Since most customers pay in a single installment, ensure checkout is frictionless, with seamless credit card and digital wallet processing. <br>
ii. Promote Installment Flexibility (9–10 range): <br>
Offer low or zero-interest EMI options in this popular range to attract mid- to high-value purchases. <br>
iii. State-Level Analysis: <br>
Investigate which states rely more on installment-based payments and design localized credit/financing promotions. <br>

5. Customer Experience & Reviews <br>
i. Leverage Review Data: <br>
a. Segment review scores by state, product category, and delivery performance. <br>
b. Identify areas where poor delivery correlates with low customer satisfaction. <br>
ii. Actively Respond to Reviews: <br>
Implement a structured customer feedback loop to acknowledge complaints, offer compensation, and improve service quality. <br>
iii. Enhance Trust via Transparency: <br>
Provide customers with accurate delivery estimates and proactive updates when delays occur. <br>

6. Data-Driven Strategic Initiatives <br>
i. Predictive Demand Forecasting: <br>
Build machine learning models using seasonal and geographic trends to forecast demand and optimize supply chain planning.
ii. Customer Segmentation (RFM Analysis): <br>
Cluster customers based on recency, frequency, and monetary value to personalize offers and improve retention. <br>
iii. Dynamic Pricing Strategy: <br>
Experiment with state-level pricing models, offering discounts in price-sensitive regions and premium bundles in high-income areas.
