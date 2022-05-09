### **SUMMARY**
# Cryptocurrency Clusters


1. Cleaned data. 
2. Discarded cryptocurrencies that are not being traded. 
3. Getting DataFrame 

![image](https://user-images.githubusercontent.com/92575973/167062157-07de518a-8207-43d0-b937-68afbe2f1527.png)



4. The data in Machine Learning should be numeric. Creating dummies variables. Getting 98 columns. 


![image](https://user-images.githubusercontent.com/92575973/167062249-8d2315a2-2eb6-4842-bc6f-0df60d1e0926.png)



5. Standardized the dataset using StandardScaler(), helping us to standardized the features by removing the mean and scaling to unit variance. Centering and scaling happen independently on each feature by computing the relevant statistics on the samples in the training set. 


![image](https://user-images.githubusercontent.com/92575973/167062292-5ebf2f7d-bc3d-4222-899b-cabe43cc8b01.png)






### Dimensionality Reduction

6. The features did not reduce significantly since we scaled the data before. 
PCA is fundamentally a dimensionality reduction algorithm, but it can also be useful as a tool for visualization, for noise filtering, for feature extraction and engineering.

![image](https://user-images.githubusercontent.com/92575973/167062331-813f7f94-03c1-4482-9d8d-e590a0c01c47.png)



7. Reducing and converting similarities between our data set with t-SNE to join probabilities and tries to minimize the Kullback-Leibler divergence between the joint probabilities of the low-dimensional embedding and the high-dimensional data. 

![image](https://user-images.githubusercontent.com/92575973/167062396-56c92498-d441-4e72-ad4e-e1cc4724610e.png)



8. We can see in the scatter plot of the t-SNE output that we have that clusters are dense in one region and 2 clusters are smaller and equidistant to each other. 

![image](https://user-images.githubusercontent.com/92575973/167062447-c9c59a58-7bdc-4af3-b00d-80b6553d4af0.png)




### Cluster Analysis with k-Means
The goal of KMeans is to identify similar data points and cluster them together while trying to distance each cluster as far as possible. Its “similarity” calculation is determined via Euclidean distance or an ordinary straight line between two points. The shorter the Euclidean distance the more similar the points are.


9.  USISING PCA METHOD = There are not clusters as we can see clearly on the plot. The data are very very different. In other words,there are not homogeneous subgroups within the data. 
 
![image](https://user-images.githubusercontent.com/92575973/167465462-62f38e20-8cbc-4dd8-9cf1-2bf5ab0737b2.png)



I wanted to include this info in the sumamry, since t_SNE is another method to reduce the dimension and was used in this homework.

9.1 USING t-SNE METHOD = The best number of clusters is 3, since initially, the quality of clustering improves rapidly when changing the value of K but eventually stabilizes. The elbow point is the point where the relative improvement is not very high anymore.

![image](https://user-images.githubusercontent.com/92575973/167062112-82ee1719-6216-4a25-a02a-3e3a78958792.png)




 
