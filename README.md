# Credit Card Behavioral Segmentation: A Data-Driven Banking Strategy

##  Problem Statement: Information Asymmetry in Finance
In the modern financial sector, banks often struggle with **Information Asymmetry**. While they possess vast amounts of transaction data, they often lack a clear understanding of the behavioral patterns of their individual customers. 

A "one-size-fits-all" approach to credit limits and interest rates leads to:
* **Market Inefficiency**: High-value customers are underserved.
* **Risk Mismanagement**: High-risk borrowers are not identified early enough.
* **Lack of Transparency**: Customers do not receive products tailored to their actual financial health.

##  The Solution: Machine Learning Behavioral Analytics
This project addresses these challenges by leveraging a dataset of ~9,000 active credit card holders. Using **Unsupervised Learning (K-Means)**, the model identifies 5 unique "financial fingerprints" based on 17 behavioral variables.

To ensure the model is transparent and interpretable, I utilized **Principal Component Analysis (PCA)** to create a **Biplot**. This visualization maps complex, 17-dimensional data into a 2D space, showing exactly which variables (like Cash Advance, Purchases, or Balance) define each customer segment.

## Project Impact
The implementation of this model provides several key benefits:
1. **Precision Banking**: Allows for personalized credit limit adjustments based on actual spending habits (PC1) versus debt reliance (PC2).
2. **Fair Pricing**: Helps in offering fairer interest rates to "Prime Transactors" while identifying "Cash-Reliant" users for targeted risk intervention.
3. **Strategic Marketing**: Enables banks to move from broad marketing to data-driven, personalized customer experiences.


##  Technical Results & Interpretation

The Biplot analysis revealed five distinct segments:
* **Cluster 1 (Prime Transactors)**: High spending, high payment frequency. Ideal for premium rewards.
* **Cluster 3 (Cash-Reliant Borrowers)**: High reliance on cash advances and debt. Requires risk monitoring.
* **Cluster 2 (Installment Shoppers)**: Prefer structured monthly payments for budget management.
* **Cluster 0 (Standard Revolvers)**: Average users who maintain a consistent balance.
* **Cluster 4 (Passive Users)**: Low-activity accounts with minimal credit utilization.

## Tech Stack
* **Language**: Python
* **Tools**: Scikit-Learn (K-Means, PCA), Seaborn, Matplotlib,
* **Data Source**: CC General Dataset (Kaggle).
