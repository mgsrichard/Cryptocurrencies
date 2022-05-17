# Cryptocurrencies
Cryptocurrencies and Unsupervised Machine Learning


The purpose of this project is to design an unsupervised machine learning model that will show how cryptocurrencies that are currently on the market can be grouped and classified. This project is done through the following four steps:

 ## Preprocessing the Data for PCA
 In this step, we cleaned the data, retaining only cryptocurrencies that are being traded, removing any rows with null values, and deleting rows where no coins have been mined. Then, the get_dummies method was used to convert text/categoric features into numeric features. Finally, the StandardScaler() function with the fit_transform method was called to normalize the data so that features that have a much wider value in range are not assigned an inappropriate level of importance by the machine learning classifier.
 ### Sample of preprocessing code
 ![Preprocessing](https://github.com/mgsrichard/Cryptocurrencies/blob/main/images/Preprocessing.png)
 ## Reducing Data Dimensions Using PCA
 In this step, we used Principal Component Analysis (PCA) to reduce the number of features to three from greater than 90 to 3. Then we created a new dataframe with the three calculated principal components to use as input for the next step.
 ![PCA](https://github.com/mgsrichard/Cryptocurrencies/blob/main/images/PCA_Code.png)
 ## Clustering Cryptocurrencies Using K-Means
 In this step, we first created an elbow curve using hvPlot so we could find the best value for K for the data produced above. This means we calculated the best number of clusters to instruct the K-Means algorithm to sort the dataset into. Then, using the K=4 value that the elbow curve produces, we used the K-Means algorithm with K=4 to predict/sort our data into clusters. This process gave us insight into one way the cryptocurrencies can be logically sorted.
 ![Elbow Curve](https://github.com/mgsrichard/Cryptocurrencies/blob/main/images/Elbow%20Curve.png)
 ![KMeans](https://github.com/mgsrichard/Cryptocurrencies/blob/main/images/KMeans_Code.png)
 ## Visualizing Cryptocurrency Results
 In this step, we used graphs and tables to visualize the results of step 3. We created a 3D scatter plot which shows the 4 clusters of cryptocurrencies. We printed out a table containing a list of tradable cryptocurrencies, and stated how many there were. Finally, we reduced the data to a two dimensional scatter plot with Total Coins Mined on the x axis and Total Coin supply on the y axis to give us another way to see how the cryptocurrency clusters were organized.

### 3-D scatter of Clusters from K Means Analysis
![3d scatter](https://github.com/mgsrichard/Cryptocurrencies/blob/main/images/3d_scatter.png)
### Table of Tradable Cryptocurrencies
![Table](https://github.com/mgsrichard/Cryptocurrencies/blob/main/images/Tradable%20currencies.png)
### 2-D Scatter of Clusters by Coin Supply Vs. Coins Mined
![2d scatter](https://github.com/mgsrichard/Cryptocurrencies/blob/main/images/2d_scatter.png)


#### Contact Information
Martha Richarson <br>
mgsrichard@yahoo.com
