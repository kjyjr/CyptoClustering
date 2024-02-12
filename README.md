# CyptoClustering

This challenge involved the use of Python and unsupervised learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

Using a Jupyter notebook, the necessary libraries and dependencies were first imported into it: Pandas and HVPlot along with KMeans, PCA, and StandardScaler from SKLearn.

Data from the source CSV file was then read and loaded into a dataframe, and summary statistics on the data observed using the .describe() operator. The data was then plotted in the form of a line graph to gain a visual of the different price change variables in the dataset.

From there, the data was scaled, and a best value for k was determined as well as the cryptocurrencies clustered using K-Means. Use of the elbow method algorithm and an accompanying elbow curve showed the best value for k to be four. Using that value, a group of four clusters was arrived at using K-Means, and an accompanying dataframe and scatter plot of the cluster values produced.

Clusters were then further optimized via Principal Component Analysis (PCA), and a dataframe of the PCA data was constructed. That data was in turn used, along with another elbow curve, to find the best value for k which also was demonstrated to be four. So both the original dataset and the PCA dataset supported a k value of four.

The PCA data was also used to cluster the cryptocurrencies with K-Means, and a scatter plot produced to show those.

Composite plots were finally presented, showing the comparison between the elbow curves using original data and PCA data and the contrast between the scatter plots that used scaled data and PCA data. The latter composite displayed the effect of using fewer features to cluster data using K-Means. By doing so, the number of data points that appeared was reduced. In contrast to the scatter plot of results with scaled data, the scatter plot of results with PCA data showed fewer data points, ones that were more narrowly clustered. But there were still four clusters/groups identified. So by using fewer features, similar performance could still be achieved with the PCA model as with the scaled one.