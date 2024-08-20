# CryptoClustering
# Cryptocurrency Clustering Analysis

## Overview
This project performs a clustering analysis on cryptocurrency market data using K-means clustering and Principal Component Analysis (PCA). The goal is to group cryptocurrencies based on their price change percentages over various time periods.

## Features
- Data preprocessing and scaling
- K-means clustering on original and PCA-transformed data
- Elbow curve analysis for optimal cluster determination
- PCA for dimensionality reduction
- Visualization of clusters using scatter plots

## Technologies Used
- Python 3.x
- pandas: for data manipulation
- scikit-learn: for K-means clustering and PCA
- hvplot: for interactive visualizations
- matplotlib: for static visualizations

## Dataset
The analysis uses a CSV file `crypto_market_data.csv` containing the following features for various cryptocurrencies:
- price_change_percentage_24h
- price_change_percentage_7d
- price_change_percentage_14d
- price_change_percentage_30d
- price_change_percentage_60d
- price_change_percentage_200d
- price_change_percentage_1y

## Key Findings
- The optimal number of clusters (k) for both original and PCA-transformed data is 4.
- PCA reduced the dimensionality of the data while preserving about 81.48% of the variance.
- Long-term price changes (particularly the 1-year change) have the strongest influence on clustering.

## How to Use
1. Ensure you have the required libraries installed:
   ```
   pip install pandas scikit-learn hvplot matplotlib
   ```
2. Place the `crypto_market_data.csv` file in a `Resources` folder in the same directory as the notebook.
3. Run the Jupyter notebook cells sequentially to perform the analysis.

## Future Improvements
- Incorporate additional features for clustering
- Experiment with other clustering algorithms
- Develop a predictive model based on the cluster assignments

## License
This project is open-source and available under the MIT License.
