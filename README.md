# crypto_clustering Data Normalization
Use StandardScaler() from scikit-learn to normalize the data from the CSV file.
Create a DataFrame with the scaled data, setting "coin_id" from the original DataFrame as the index.
Finding the Optimal k-Value
Use the elbow method to find the best k-value:
Create a list of k-values from 1 to 11.
Calculate and store the inertia for each k.
Plot the inertia values to visually identify the optimal k.
Answer: What is the best value for k?
K-means Clustering
Cluster cryptocurrencies using K-means with the optimal k-value:
Initialize and fit the K-means model with the original scaled data.
Predict clusters and add them to a copy of the original DataFrame.
Create an hvPlot scatter plot using "price_change_percentage_24h" and "price_change_percentage_7d", coloring by clusters, and adding "coin_id" to hover.
PCA and K-means Clustering
Perform PCA on the scaled data to reduce features to 3 components.
Calculate and analyze the explained variance:
Answer: What is the total explained variance of the three principal components?
Repeat the elbow method and K-means clustering using PCA data:
Find the best k-value with the PCA data.
Cluster the data using K-means and create a scatter plot using "PC1" and "PC2".
Answer: What is the best k-value with PCA data? Does it differ from the original data?
Answer: What is the impact of using fewer features for clustering?
