# Beyond the Metal Tiers: A K-Means Analysis of FL Health Plans
*An exploratory public-health analytics project.*

This project explores cost-sharing patterns within 2026 Florida ACA Marketplace health insurance metal levels using K-means clustering to identify differences in deductibles and out-of-pocket maximums. 

## Quick Links
- [CMS Source]([https://google.com](https://www.cms.gov/marketplace/resources/data/public-use-files?utm_source=chatgpt.com))

## What this demonstrates
- Data cleaning, preprocessing, and missing value handling
- Elbow method utilization for optimal K selection
- Comparative analysis of cost-sharing structures within metal levels
- Scatterplot visualization of clusters and centroids

## Dataset Snapshot
- **2,201** unique plans
- **26** unique insurance issuers
- **Metal Levels**: Bronze, Expanded Bronze, Silver, Gold, and Platinum
- **Primary Variables**: MetalLevel, TEHBDedInnTier1Individual, TEHBInnTier1IndividualMOOP, TEHBDedInnTier2Individual, and TEHBInnTier2IndividualMOOP

## Methods At A Glance

| Analysis | Tools Used | Purpose |
|---|---|---|
| Data Cleaning & Preprocessing | Python, Pandas, NumPy | Filter ACA plans, handle missing values, and prepare numerical variables |
| Exploratory Data Analysis | Pandas, Matplotlib | Examine deductible and out-of-pocket maximum distributions |
| Feature Selection | Pandas | Select relevant cost-sharing variables for clustering |
| K-Means Clustering | Scikit-learn | Identify groups of plans with similar cost-sharing structures |
| Cluster Evaluation | Scikit-learn | Evaluate cluster assignments and compare K values using elbow method |
| Metal-Level Comparison | Pandas, Scikit-learn | Analyze clustering results within individual metal levels |
| Data Visualization | Matplotlib | Create scatterplots displaying clusters and centroids |

