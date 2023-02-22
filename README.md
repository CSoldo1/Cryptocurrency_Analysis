# Overview
Accountability Accounting, a prominent investment bank, is interested in offering a new cryptocurrency investment portfolio for its customers. The company, however, is lost in the vast universe of cryptocurrencies. They have asked me to create a report that includes what cryptocurrencies are on the trading market and how they could be grouped to create a classification system for this new investment. Because there is no known output that that the investment firm is looking for, I have decided to use unsupervised learning, specifically, a clustering algorithm. 

## Resources
*Data: crypto_data.csv
*Software: Jupyter Notebook

## Analysis
To begin, I removed all rows that contained null or missing values. I only kept the cryptocurrencies that were actively being traded. I then removed certain columns that were not pertinent to the analysis. I created dummy variables for the 'Algorithm' and 'ProofType' columns. Then, I used the fit_transform() function to standardize the features in the data. Using the newly created dataframe, I applied PCA to reduce the dimensions to three prinicpal components. The results of the PCA algorithm were concatenated into their own data frame (pcs_df). I then used the pcs_df dataframe to run the K-means algorithm to make predicitons of the K clusters for the cryptocurrencies' data. Finally, I created a 3D scatter plot to help visualize how the cryptocurrencies clustered in multidimensional space. 

## Results

