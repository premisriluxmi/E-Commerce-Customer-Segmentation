# E-Commerce Customer Segmentation & Recommendation Analysis

## Project Overview

This project analyzes e-commerce customer purchasing behavior using the UCI Online Retail dataset. It applies RFM analysis and K-Means clustering to identify meaningful customer segments and uses Cosine Similarity to recommend similar products.

The main objective is to understand customer behavior, identify valuable customer groups, and provide data-driven business recommendations.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Workflow

### Day 1 – Data Understanding and Cleaning
- Explored the Online Retail dataset.
- Identified missing values and duplicate records.
- Removed cancelled transactions.
- Removed invalid quantities and unit prices.
- Created a TotalAmount feature.

### Day 2 – RFM Analysis
Created three customer-level features:
- Recency – How recently a customer purchased.
- Frequency – How often a customer purchased.
- Monetary – How much a customer spent.

Applied log transformation and feature scaling.

### Day 3 – Customer Segmentation
- Evaluated different K-Means cluster counts.
- Applied K-Means clustering with four clusters.
- Visualized customer groups using PCA.
- Created customer segment profiles.

### Day 4 – Product Recommendation
- Created a customer-product purchase matrix.
- Calculated product similarity using Cosine Similarity.
- Developed a function to recommend similar products.

### Day 5 – Business Analysis
- Analyzed customer segment distribution.
- Compared revenue contributions.
- Created business strategies for each segment.
- Saved final analysis outputs.

## Dataset

**Source:** UCI Machine Learning Repository – Online Retail Dataset

https://archive.ics.uci.edu/dataset/352/online+retail

Original dataset: 541,909 records.

After cleaning:
- Transactions: 392,692
- Customers: 4,338
- Products: 3,665
- Countries: 37

## Customer Segments

| Segment | Description |
|---|---|
| Champions | Recent, frequent, high-spending customers |
| At-Risk Customers | Customers who have not purchased recently |
| Recent Occasional Buyers | Recent customers with lower purchase frequency |
| Regular Customers | Customers with moderate purchase frequency and spending |

## Revenue Analysis

| Customer Segment | Revenue Contribution |
|---|---:|
| Champions | 64.89% |
| Regular Customers | 23.64% |
| At-Risk Customers | 6.22% |
| Recent Occasional Buyers | 5.25% |

Champions contribute the largest share of revenue, highlighting the importance of customer retention strategies.

## Product Recommendation

Cosine Similarity was used to identify products with similar customer purchasing patterns.

The recommendation function returns the top five similar products for a selected product.

## Business Recommendations

- Champions: Loyalty rewards and exclusive offers.
- At-Risk Customers: Personalized discounts and win-back campaigns.
- Recent Occasional Buyers: Product bundles and related recommendations.
- Regular Customers: Loyalty points and repeat-purchase offers.

## Project Outputs

- `online_retail_day1_cleaned.csv`
- `customer_rfm_features.csv`
- `customer_segmentation_results.csv`
- `final_customer_segmentation.csv`
- `revenue_analysis.csv`
- `business_strategies.csv`

## Conclusion

This project demonstrates how data analysis and unsupervised machine learning can help businesses understand customer purchasing behavior, identify customer segments, recommend similar products, and develop effective marketing strategies.