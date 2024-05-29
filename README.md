# CryptoClustering
Module 19 Challenge - Unsupervised Learning
# CryptoClustering

## Project Overview

Cryptocurrency markets are known for their volatility and rapid price changes. Understanding how different cryptocurrencies react to these changes can provide valuable insights for investors and analysts. This project employs unsupervised learning techniques to analyze and cluster cryptocurrencies based on their 24-hour and 7-day price changes.

By utilizing clustering algorithms and Principal Component Analysis (PCA), we aim to uncover patterns and groupings within the crypto market data. This analysis helps in identifying whether short-term and medium-term price movements significantly influence the clustering behavior of different cryptocurrencies.

## Key Objectives

1. **Data Normalization:** Standardize the cryptocurrency market data to ensure all features contribute equally to the clustering process.
2. **Optimal Clustering with Elbow Method:** Determine the best number of clusters (k) using the elbow method to achieve meaningful groupings.
3. **K-Means Clustering Analysis:** Apply K-means clustering to the normalized data and visualize the groupings based on price change percentages.
4. **Dimensionality Reduction with PCA:** Reduce the feature space to three principal components and analyze the impact on clustering performance.
5. **Comparison and Visualization:** Compare the clustering results from the original data and the PCA-transformed data to understand the effect of dimensionality reduction.

## Methodology

### 1. Data Preparation
- Load the `crypto_market_data.csv` dataset.
- Generate summary statistics and visualizations to understand the data distribution.
- Normalize the data using `StandardScaler` to standardize the feature scales.

### 2. Elbow Method for Optimal k
- Implement the elbow method to find the optimal number of clusters.
- Plot inertia values for k ranging from 1 to 11 and visually identify the "elbow point."

### 3. K-Means Clustering
- Initialize the K-means model with the optimal k value.
- Fit the model to the normalized data and predict cluster assignments.
- Visualize the clusters using `hvPlot`, with 24-hour and 7-day price changes as axes.

### 4. Principal Component Analysis (PCA)
- Perform PCA to reduce the dataset to three principal components.
- Calculate the explained variance to assess the significance of each principal component.
- Reapply the elbow method to the PCA-transformed data to find the new optimal k value.
- Cluster the PCA-transformed data and visualize the clusters.

### 5. Results Comparison
- Create composite plots to compare elbow curves from the original and PCA data.
- Overlay scatter plots of clusters obtained from both datasets.
- Analyze how reducing the number of features impacts the clustering results.

## Results and Insights

- **Optimal k Values:** Identify the optimal number of clusters using both original and PCA data.
- **Cluster Visualization:** Visualize how cryptocurrencies group based on their price changes over different periods.
- **Impact of PCA:** Evaluate the effectiveness of PCA in simplifying the data while retaining essential patterns.

## Conclusion

This project demonstrates the application of unsupervised learning techniques to analyze cryptocurrency market behavior. By comparing clustering results from original and PCA-transformed data, we gain insights into the influence of dimensionality reduction on clustering performance. This analysis helps in understanding the key factors driving price changes and their impact on the market structure.

## Contributing

Contributions to this project are welcome! Feel free to fork the repository, make improvements, and submit a pull request.

