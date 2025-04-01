# Project 1: e-Commerce (Target) Sales Dataset Analysis
## Project Overview
For this project, I will find the top three states in Brazil with the most orders. I will analyze the purchasing behavior of these states.
## Dataset Information
- **Dataset Name**: e-Commerce (Target) Sales Dataset
- **Dataset Source**: Kaggle
- **Dataset URL**: [e-Commerce (Target) Sales Dataset](https://www.kaggle.com/datasets/devarajv88/target-dataset/data?select=products.csv)
- **Dataset Description**: This dataset contains 7 different csv files with information about customers and their online purchases from Target in Brazil. The following csv files will be used in this project: 'customers.csv', 'orders.csv', 'payments.csv', 'products.csv', and 'order_items.csv'.
- **Author**: Devaraj V
- **Citations**: No citations were provided.
- **Licensing and Usage**: In the licensing section, this dataset is classified as 'Other (specified in description)'. There is no description provided or any other mention of licensing.
## Main Question
What are the top 3 states with the most orders, and what was their purchasing behavior?
## Dataset Structure
The 5 csv files have the following columns. I will only be using the bolded columns.

1. **customers.csv**
- **customer_id**: ID of the consumer who made the purchase
- customer_unique_id: Unique ID of the consumer
- customer_zip_code_prefix: Zip Code of consumer’s location
- customer_city: Name of the City from where order is made
- **customer_state**: State Code from where order is made (Eg. são paulo - SP)

2. **orders.csv**
- **order_id**: A Unique ID of order made by the consumers
- **customer_id**: ID of the consumer who made the purchase
- order_status: Status of the order made i.e. delivered, shipped, etc.
- **order_purchase_timestamp**: Timestamp of the purchase
- order_delivered_carrier_date: Delivery date at which carrier made the delivery
- order_delivered_customer_date: Date at which customer got the product
- order_estimated_delivery_date: Estimated delivery date of the products

3. **payments.csv**
- **order_id**: A Unique ID of order made by the consumers
- payment_sequential: Sequences of the payments made in case of EMI
- **payment_type**: Mode of payment used (Eg. Credit Card)
- **payment_installments**: Number of installments in case of EMI purchase
- **payment_value**: Total amount paid for the purchase order

4. **products.csv**
- **product_id**: A Unique identifier for the proposed project
- **product_category_name**: Name of the product category
- product_name_lenght: Length of the string which specifies the name given to the products ordered
- product_description_length: Length of the description written for each product ordered on the site
- product_photos_qty: Number of photos of each product ordered available on the shopping portal
- product_weight_g: Weight of the products ordered in grams
- product_length_cm: Length of the products ordered in centimeters
- product_height_cm: Height of the products ordered in centimeters
- product_width_cm: Width of the product ordered in centimeters

5. **order_items.csv**
- **order_id**: A Unique ID of order made by the consumers
- order_item_id: A Unique ID given to each item ordered in the order
- **product_id**: A Unique ID given to each product available on the site
- seller_id: Unique ID of the seller registered in Target
- shipping_limit_date: The date before which the ordered product must be shipped
- **price**: Actual price of the products ordered
- freight_value: Price rate at which a product is delivered from one point to another






## Data Cleaning
The dataset was cleaned by performing the following:
- **Handling 0 values**: Replaced the 0 values with the median or used K-Nearest Neighbors.
- **Checked for missing values**: None were found.
- **Checked for duplicate rows**: None were found.
- **Examined data types**: The data types did not need to be adjusted.
- **Examined numerical data**: Reviewed distributions and outliers. Many outliers were kept. Without additional domain knowledge, there is not much justification to remove what are suspected to be outliers.
## Exploratory Data Analysis
I examined the potential relationships within the data through:
- **Correlation matrix and heatmap**: I found that 'Glucose', 'BMI', and 'Age' had the highest correlation to 'Outcome'.
- **Visualizations**: Through histograms, boxplots, and scatterplots I examined the relationships between different columns and the diabetes outcome.
## Findings
- **Glucose**: Higher glucose levels are associated with a patient having diabetes.
- **BMI**: A higher BMI is associated with a patient having diabetes.
- **Age**: Age is also a key indicator of a patient potentially having diabetes.
## Visualizations
I created a dashboard on Tableau Public with visualizations of the key findings.
[Tableau Dashboard](https://public.tableau.com/views/Project2DiabetesDatasetAnalysis/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)
## Conclusion
- **Key Takeaways**: Higher glucose levels, BMI, and age are the strongest indicators of diabetes diagnosis.
- **Limitations**: The 'SkinThicknes' (227) and 'Insulin' (374) columns had many 0 values.
