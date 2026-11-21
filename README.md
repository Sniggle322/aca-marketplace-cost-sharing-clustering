# Beyond the Metal Tiers: A K-Means Analysis of FL Health Plans
*An exploratory public-health analytics project.*

This project explores cost-sharing patterns within 2026 Florida ACA Marketplace health insurance metal levels using K-means clustering to identify differences in deductibles and out-of-pocket maximums. 

## Quick Links
- [CMS Source](https://www.cms.gov/marketplace/resources/data/public-use-files)
  
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

## Why this matters
Health insurance plans often come with many different options for customers to choose from. The objective of this project is to use data from the ACA Marketplace plans in Florida in order to discover and characterize health insurance patterns to better understand the options for customers. Plans offered through the Florida ACA Marketplace are categorized into five metal tiers - Bronze, Expanded Bronze, Silver, Gold, and Platinum with Bronze containing the lowest level insurance plans and Platinum having the highest level insurance plans. The main goal of this project is to investigate using machine learning concepts and models in order to answer the question “What distinct deductible and out-of-pocket maximum patterns exist with metal levels among Florida ACA Marketplace plans in 2026?”. The general prediction for these plans is that the lower level plans would tend to have higher deductible rates and customers would have to pay higher out of pocket costs.

## Visualizations


## Adaptations or Modifications
While clustering the Platinum metal level, it was discovered that only 1 unique cost sharing combination existed. This prompted further exploration, revealing that overfiltering of missing values  created unclusterable data points. Unlike the other metal levels, Platinum plans often have $0 deductibles. Hence, explaining the large number of missing/nonapplicable values within this metal level. Consequently, the missing values were replaced with $0, uncovering 3 distinct clusters of varying MOOP costs and fixed $0 deductible. 

## Findings
Across lower metal tiers, the maximum out of pocket rates cap out around $10,000 showing that insurers have a standard out of pocket rate capping out at $10,000. There are very distinct patterns within every metal tier showing that each metal tier has a standard ratio, the Platinum tier being the highest level, the individual deductible rate is $0,  as the tier levels go down, the individual maximum out of pocket cost goes up and caps out at around $10,000. This shows that as the Metal Tiers shift downwards, the insurance companies take less responsibilities on the bill and the consumer is then handed that responsibility on the medical cost. By comparing the two lowest level tiers (Expanded Bronze and Bronze), an out-of-pocket cap at around $10,000 appears, but, there is a shift between the two tiers, due to the Expanded Bronze tier having more plans, there is a distinct lower deductible group that the Bronze tier does not have showing more flexibility than the Bronze tier.


