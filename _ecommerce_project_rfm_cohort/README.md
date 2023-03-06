# 📈 Brazil E-commerce // Project

## Description

This is one of the main projects from the Data Analyst course from [Karpov.Courses](https://external.ink?to=/https://karpov.courses/analytics) that I enrolled in June 2022. In this project we used a brazil e-commerce dataset. The main idea of the project is to learn to view data holistically, draw conclusions based on available data, and apply a customer segmentation approach, such as RFM analysis


## Project Tasks

1.  How many users have made a single purchase?
    
2.  On average, how many orders are not delivered due to various reasons (Make a detailed breakdown of reasons)?
    
3.  For each product, determine the day of the week on which the product is most frequently bought
    
4.  What is the average number of purchases per customer per week (in month)? Please note that within a month, the number of weeks may not be a whole number. For example, November 2021 had 4.28 weeks
    
5.  Using pandas, perform a cohort analysis of customers for the period from January to December and identify the cohort(s) with the highest retention for the 3rd month.
    
6.  "Frequently, for high-quality analysis of audience, segmentation-based methods are used. Use Python to perform RFM segmentation of customers in order to make a high-quality evaluation of the audience. For clustering, you can use the following metrics: R (Recency) - time elapsed since the last purchase before the current date, F (Frequency) - total number of purchases made over time, and M (Monetary) - total amount spent over time.


## About RFM analysis

Customer segmentation is important for multiple reasons. We get a deeper knowledge of our customers and can tailor targeted marketing campaigns.

The RFM method was introduced by Bult and Wansbeek in 1995 and has been successfully used by marketers since.  
It analyzes customers' behavior on three parameters:  
**Recency**: How recent is the last purchase of the customer.  
**Frequency**: How often the customer makes a purchase.  
**Monetary**: How much money does the customer spends.

The advantages of RFM is that it is easy to implement and it can be used for different types of business. It helps craft better marketing campaigns and improves CRM and customer's loyalty.

The disadvantages are that it may not apply in industries where customers are usually one time buyers. It is based on historical data and won't give much insight about prospects.

## Methodology of RFM analysis

To get the RFM score of a customer, we need to first calculate the R, F and M scores on a scale from 1 (worst) to 5 (best).

1.  calculate Recency = number of days since last purchase
2.  calculate Freqency = number of purchases during the studied period (usually one year)
3.  calculate Monetary = total amount of purchases made during the studied period
4.  find quintiles for each of these dimensions
5.  give a grade to each dimension depending in which quintiles it stands
6.  combine R, F and M scores to get the RFM score
7.  map RF scores to segments

## Used methods and framework

In this case i used methods from **Pandas, Seaborn, Statistics, Datetime andNumpy** libraries, such as:

`pd.to_datetime`, 
`.dtypes`, 
`dt.strftime('%A')`
`.groupby()`, `.agg()`
`.nlargest()`
`.astype()`
`.np.arange()`
`.unstack()`
`.first()`
`.dt.day_name()`
`.mul()`
`.reset_index()`
`.idxmax()`, 
`.sort_values()`, 
`.quantile()`
`.map()`
`.pd.read\_csv()` with `parse_dates` parametr
`.sns.set_palette()`, `sns.barplot()`, `sns.countplot()`



## Dataset Fields:

**olist_customers_datase.csv** — dataset of unique customer:
| name | description |
| ---- | ----------- |
| customer_id | id of customer for each order
| customer_unique_id | unique id of customer
| customer_zip_code_prefix | zip-code
| customer_city | city of delivery
| customer_state | state of delivery

**olist_orders_dataset.csv** — orders dataset:
| name | description |
| ---- | ----------- |
| order_id |  unique order id
| customer_id | id of customer for each order
| order_status | order status
| order_purchase_timestamp | time/date of purchase
| order_approved_at | time/date of approving order
| order_delivered_carrier_date |time/date of issuance for logistic-partner
| order_delivered_customer_date | time/date of delivery 
| order_estimated_delivery_date | estimated_delivery time/date

**olist_order_items_dataset.csv** — items in order
| name | description |
| ---- | ----------- |
| order_id | unique order id (check)
| order_item_id | id inside one order
| product_id | product id (barcode)
| seller_id | id of distributor
| shipping_limit_date | maximum date for delivery, before order will be giving to logistic-partner
| price | price per unit
| freight_value | weight of product 


## Contact

* Connect with me on:   
    📜 [Email](mailto:alexey.golovin@gmail.com)   
    🏦 <a href="https://www.linkedin.com/in/alexey-golovin/">LinkedIn</a>   
