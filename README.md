# 📊 Marketing Campaign Clustering Analysis

A Data Science project aimed at analyzing a marketing campaign dataset using clustering techniques like K-Means and Gaussian Mixture Models (GMM).

## 📖 Table of Contents

- Introduction
- Features
- Data Preprocessing
- Clustering Analysis
- Acknowledgements

## 🌟 Introduction

This project analyzes customer data from a marketing campaign. Dataset available in this repo.
The goal is to:
1. Segment customers using clustering algorithms.
2. Identify customer groups.
3. Assess the effectiveness of the campaigns

## ✨ Features

- **Data Preprocessing**: Handling missing values, encoding categorical features, and scaling numeric data.
- **Exploratory Data Analysis (EDA)**: Visualizing key features and relationships within the dataset.
- **Dimensionality Reduction**: Using PCA to reduce data dimensionality and visualize clusters in 2D space.
- **Clustering Techniques**: Applying both K-Means and GMM to group customers into clusters.
- **Optimal Cluster Selection**: Using the Elbow Method, AIC, and BIC to determine the best number of clusters.
- **Clustering Evaluation**: Assessing clustering performance using Silhouette Score, Homogeneity, and other metrics.
- **Custom Metrics**: Calculating distances to cluster centers to assess how well the data points fit within their clusters.

## 📚 Data Preprocessing

The dataset includes customer demographics, product purchases, and campaign responses. 
Data preprocessing includes handling missing values, encoding categorical features, and scaling numeric variables for clustering.

## 🔍 Clustering Analysis

The number of clusters was identified using the AIC, BIC and Elbow methods as explained in section 3. The final number of optimal clusters was 4. The specific hyperparameters of the clustering models were not changed further.
K-Means and Gaussian Mixture Models (GMM) were applied to segment customers.
The accompanying Voronoi diagram further emphasises the area covered by each cluster, revealing that the final section represents the largest group.

![Voronoi diagram](https://github.com/user-attachments/assets/482a2622-9f60-449c-921f-aee134f8c127)

This visualisation effectively shows the spatial distribution and relative sizes of the clusters. 
The GMM algorithm had a Silhouette score of 0.4095 while the K-Means had a score of 0.4772, highlighting the better performance of the K-Means algorithm in terms of cluster cohesion and separation. 
This suggests that the K-Means clustering produced groups that were more internally homogeneous and externally differentiated compared to those identified by the GMM algorithm. 
Other metrics to take into consideration were Completeness and Homogeneity. 
GMM had a Completeness score of 1.0 and a Homogeneity score of 1.0 while K-Means had a Completeness score of 0.9262 and a Homogeneity score of 0.9193, this shows that the GMM algorithm was superior in terms of both Completeness and Homogeneity, achieving perfect scores.
This indicates that all members of a given class were assigned to the same cluster (Completeness), and each cluster contains only members of a single class (Homogeneity).

## 🙏 Acknowledgements

- **Akash Patel** for making the dataset available on Kaggle: https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis 
