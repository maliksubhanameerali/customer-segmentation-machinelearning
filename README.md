# Customer Segmentation using K-Means Clustering

## Overview
This project applies K-Means clustering to segment customers into distinct groups based on income, spending behavior, purchase recency, and shopping channel activity. The goal is to identify actionable customer profiles that can inform targeted marketing strategies.

## Dataset
The dataset contains customer records including demographic information (age, income) and behavioral data (spending, purchase frequency, recency, and website/in-store activity).

## Tools Used
- Python
- pandas, numpy
- scikit-learn (KMeans, StandardScaler)
- matplotlib / seaborn

## Approach
1. Data cleaning and preprocessing
2. Feature scaling with StandardScaler
3. Used the Elbow Method to determine the optimal number of clusters
4. Applied K-Means clustering (k=6)
5. Profiled and interpreted each segment based on income, spending, recency, and purchase channel behavior

## Results

Six distinct customer segments were identified:

| Cluster | Segment Name | Characteristics |
|---|---|---|
| 0 | Loyal High-Value Customers | High income, high spending, frequent online and in-store purchases, average recency |
| 1 | Conservative Traditional Shoppers | Oldest customers, moderate income, low spending, few purchases |
| 2 | Premium Active Customers | High income, highest spending, very recent purchases, few website visits |
| 3 | At-Risk Premium Customers | High income, very high spending, but long time since last purchase |
| 4 | Inactive Budget Customers | Lower income, low spending, infrequent and non-recent purchases |
| 5 | Price-Conscious Browsers | Youngest customers, lowest income and spending, frequent website visits but few purchases |

**Key insight:** Premium Active Customers (Cluster 2) and At-Risk Premium Customers (Cluster 3) both spend heavily, but Cluster 3's high recency suggests a targeted re-engagement campaign could recover significant revenue from previously high-value customers who have gone quiet.

## How to Run
1. Clone this repo
   ```bash
   git clone <your-repo-url>
