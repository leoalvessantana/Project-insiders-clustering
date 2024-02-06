# Insiders Clustering

Project from Data Science Community, mentoring by Meigarom Lopes.

The business problem is selecting customers to create a loyalty program called Insiders. A UK-based online retail store has captured the sales data for different products for the period of one year (Nov 2016 to Dec 2017). The organization sells gifts primarily on the online platform. The customers who make a purchase consume directly for themselves. There are small businesses that buy in bulk and sell to other customers through the retail outlet channel.

## 1. Business Problem

Find significant customers for the business who make high purchases of their favorite products. The organization wants to roll out a loyalty program, called Insiders, to the high-value customers after identification of segments.


## 2. Data

The data used in this project can be found at [Kaggle](https://www.kaggle.com/vik2012kvs/high-value-customers-identification).


<details><summary>Click here to see the original attibutes table</summary><br>
  
Attribute | Definition
------------ | -------------
|InvoiceNo   | Invoice number (A 6-digit integral number uniquely assigned to each transaction)    |
|StockCode   | Product (item) code   |
|Description | Product (item) name   |
|Quantity    | The quantities of each product (item) per transaction   |
|InvoiceDate | The day when each transaction was generated   |
|UnitPrice   | Unit price (Product price per unit)   |
|CustomerID  | Customer number (Unique ID assigned to each customer)   |
|Country     | Country name (The name of the country where each customer resides)   |
</details>


## 3. Business Assumptions.

- Indicate customers who will be part of a loyalty program called Insiders.
- What are the main characteristics of these customers? Ticket, bascket size, high LTV, churn probability,high TVC prevision, purchasing propensity, age, location.
- How many customers will be part os this group?
- RFM model (recency, frequency,, monetary): sorted data to have a RFM Score.

## 4. Solution Strategy

0. Tools

1. Data Description: rename columns, check NA values, change types.

2. Feature Engineering: recency, frequency, monetary, gross revenue.

3. Cluster Analysis: Visualization Inspection, UMAP -t-SNE

4. Feature Engineering: create new attributes based on the original variables using mindmap hypothesis.

5. Exploratory Data Analysis (EDA): univariate and bivariate analysis. Embedding space study with PCA, UMAP, t-SNE, Decision Tree.

6. Hyperparameter Fine Tuning: K-Means, GMM, Hierarchical Clustering.

7. Deploy Database Sqlite: insiders_db.sqlite