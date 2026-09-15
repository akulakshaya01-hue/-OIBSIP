# Customer Segmentation Analysis

## Internship
Oasis Infobyte – Data Analytics Internship

## Task
Level 1 – Task 2: Customer Segmentation Analysis

## Objective
Perform customer segmentation using RFM (Recency, Frequency, and Monetary) analysis and K-Means clustering to identify distinct customer groups and support targeted marketing strategies.

## Tools & Technologies
- Python
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook / Google Colab

## Dataset
The analysis uses the Online Retail dataset containing transaction-level information such as invoice number, product details, quantity, invoice date, unit price, customer ID, and country.

## Data Preparation
- Inspected the dataset structure, data types, and missing values.
- Removed records with missing CustomerID and Description.
- Removed cancelled transactions.
- Converted InvoiceDate into datetime format.
- Calculated TotalPrice as Quantity × UnitPrice.

## RFM Analysis
Customer behaviour was measured using three key features:

- **Recency:** Number of days since the customer's most recent purchase.
- **Frequency:** Number of unique invoices associated with the customer.
- **Monetary:** Total amount spent by the customer.

## Clustering Method
- Standardized the RFM features using StandardScaler.
- Used the Elbow Method to determine a suitable number of clusters.
- Applied K-Means clustering with **4 clusters**.
- Visualized the resulting customer segments using scatter plots.
- Analyzed the average RFM values of each cluster.

## Customer Segments

| Cluster | Customer Segment |
|---|---|
| Cluster 0 | Loyal High-Value Customers |
| Cluster 1 | At-Risk / Inactive Customers |
| Cluster 2 | VIP Customers |
| Cluster 3 | Regular Customers |

## Key Insights
- Cluster 3 is the largest customer segment with 3,053 customers.
- Cluster 1 contains 1,062 customers and shows high recency with relatively low frequency and spending.
- Cluster 0 contains 211 customers with high purchase frequency and monetary value.
- Cluster 2 is the smallest segment with only 13 customers but has exceptionally high purchase frequency and monetary value.
- RFM analysis clearly distinguishes customers based on purchasing behaviour.

## Marketing Recommendations

1. **Loyal High-Value Customers:** Provide loyalty rewards, personalized offers, and early access to products.
2. **At-Risk / Inactive Customers:** Use re-engagement campaigns, reminders, and personalized discounts.
3. **VIP Customers:** Provide exclusive benefits, premium service, and VIP membership programs.
4. **Regular Customers:** Use targeted promotions and product recommendations to increase purchase frequency.

## Files
- `Task_2_Customer_Segmentation.ipynb` – Complete Jupyter Notebook containing the analysis.
- `01_elbow_method.png` – Elbow Method visualization.
- `02_recency_vs_monetary.png` – Recency vs Monetary cluster visualization.
- `03_frequency_vs_monetary.png` – Frequency vs Monetary cluster visualization.
- `04_customers_per_cluster.png` – Customer distribution by cluster.
