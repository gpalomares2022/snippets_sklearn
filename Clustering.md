# Clustering
This is a repo to take notes about how to work with ML Clustering in Sklearn

## Preparing data
````python

#Input
X=df[['col1','col2']] # pandas Dataframe
#No Labels

````
## K-means
````python
from sklearn.cluster import KMeans
kmeans= KMeans(n_clusters=3)  #Se decide 3 cluster
kmeans.fit(X)
plt.scatter (df['col1'], df['col2'], c=kmeans.predict(X)) #Pintamos los clusters
plt.scatter (kmeans.cluster_centers_[:,0], kmeans.cluster_centers_[:,1], c='red', marker='*', s= 80)   #Pintamos los centroides
plt.xlabel('Col 1')
plt.ylabel('Col 2')
````



