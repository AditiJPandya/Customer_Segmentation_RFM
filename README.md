Customer Segmentation Using RFM Analysis and K-Means
This project applies RFM (Recency, Frequency, Monetary) analysis and K-Means clustering to segment customers based on their purchasing behaviour. The objective is to identify meaningful customer groups and derive actionable business insights that can support marketing, retention, and customer relationship strategies.

Project Overview
The dataset contains transactional records including invoice numbers, product details, quantities, pricing, customer IDs, and timestamps. Using this data, the project performs:
Data cleaning and preprocessing
Feature engineering to compute RFM metrics
Scaling of features for clustering
Elbow method to determine optimal cluster count
K-Means clustering
Interpretation of segment behavior
Business recommendations based on clusters

Tools and Technologies
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-Learn
Google Colab

Methodology
1. Data Cleaning
Removed cancelled invoices
Filtered out negative and zero quantities and prices
Converted InvoiceDate to datetime format
Handled missing values appropriately
Created a filtered dataset for customers with valid Customer IDs

2. Feature Engineering
Computed RFM metrics:
Recency: Days since the customer’s last purchase
Frequency: Number of unique invoices per customer
Monetary: Total amount spent (Quantity × Unit Price)

3. Scaling
Standardized RFM features using StandardScaler to prepare for K-Means clustering.

4. Clustering
Used the Elbow Method to select the optimal number of clusters (k = 4)
Applied K-Means to segment customers
Labeled clusters based on average RFM values

5. Visualization
Created multiple plots to understand customer behaviour:
Distribution plots for Recency, Frequency, Monetary
Scatter plots for visualizing clusters
Heatmap summarizing cluster characteristics

Customer Segments Identified
Segment 1: High-Value Customers
Very recent purchases
High frequency of transactions
High monetary value
Recommendation: Implement premium loyalty programs, offer exclusive access, and provide personalized communication.

Segment 2: Loyal Customers
Active and frequent buyers
Significant revenue contribution
Recommendation: Encourage higher basket size through bundles and cross-selling.

Segment 3: Regular Customers
Moderate recency
Low spending and lower frequency
Recommendation: Use targeted promotions and reminders to increase engagement.

Segment 4: At-Risk Customers
High recency (long time since last purchase)
Low frequency and low spending
Recommendation: Launch win-back campaigns, time-limited discounts, and reactivation emails.

Key Insights
A small group of customers contributes disproportionately to total revenue.
Retention strategies for high-value and loyal customers can significantly impact profitability.
Regular and at-risk customers require targeted marketing to improve engagement.
RFM analysis converts raw transaction logs into actionable customer intelligence.

Repository Structure
Customer-Segmentation-RFM/
│
├── notebooks/
│   └── Customer_Segmentation_RFM.ipynb
│
├── images/
│   ├── recency.png
│   ├── frequency.png
│   ├── monetary.png
│   ├── cluster_scatter.png
│   └── cluster_heatmap.png
│
└── README.md

How to Use
Open the notebook in Google Colab or Jupyter Notebook.
Upload the dataset (Online Retail dataset).
Run each cell sequentially.
Modify cluster counts or visualizations as needed.

Author
Aditi Pandya
Data Analytics & Business Insights
GitHub:
