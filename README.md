Cryptocurrency Market Data Clustering with K-Means
Project Overview
This project applies clustering techniques to cryptocurrency market data to identify meaningful groupings of cryptocurrencies based on their price change percentages. The goal is to explore how K-Means clustering performs on both the original scaled data and the data reduced using Principal Component Analysis (PCA).

Dataset
The dataset used for this analysis contains various features related to cryptocurrency price changes over different time periods. The main columns used for clustering include:

price_change_percentage_24h
price_change_percentage_7d
Additional numerical features
The dataset is sourced from publicly available cryptocurrency data.

Steps Involved
Data Preprocessing:

The raw dataset is loaded and cleaned.
Numerical features are scaled using StandardScaler to standardize the data for clustering.
K-Means Clustering:

K-Means is applied to the original scaled data to group cryptocurrencies based on their market performance.
The optimal number of clusters (k) is determined using the Elbow Method.
Principal Component Analysis (PCA):

PCA is used to reduce the dimensionality of the data, transforming the features into three principal components (PC1, PC2, PC3).
K-Means clustering is then applied to the reduced data to explore how dimensionality reduction affects the clustering results.
Comparison of Clustering Results:

A composite plot contrasts the clustering results from both the original data and PCA-reduced data.
The impact of using fewer features is analyzed by comparing the distinctiveness of the clusters.
Visualization:

Scatter plots visualize the clusters in both the original and PCA-reduced data spaces, with points colored by their cluster labels.
An Elbow curve is plotted to identify the optimal value for k.
Key Insights
Using fewer features through PCA helps simplify the data, but can lead to a loss of important information, which may affect cluster accuracy.
Clustering with PCA-reduced data provides faster results and clearer visualizations but may not always capture the underlying patterns as well as the full feature set.
The optimal number of clusters (k) is determined through the Elbow Method and may vary slightly depending on the dimensionality of the data.
Technologies Used
Python
Pandas
Scikit-learn
Matplotlib
hvPlot (for interactive plotting)
Conclusion
This analysis highlights the trade-offs between using full-featured data versus reduced-dimensionality data for clustering. The findings can be used to improve decision-making or provide insights into the dynamics of the cryptocurrency market.

Feel free to adjust the content based on your specific project details and findings! Let me know if you need any changes.








