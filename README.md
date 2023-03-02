# snippets_sklearn
This is a repo to take notes about how to work with ML in Sklearn
## Preparing data
````python

#Input
X= df[['TotalSF']] # pandas Dataframe
#labels
y= df[['SalesPrice']] #pandas Series

````
## K-means
````python

from sklearn.cluster import KMeans

kmeans= KMeans(n_clusters=3)  #DECIDO QUE HAY 3 CLUSTERES..PORQUE LO CREO.
X=players[['power_stamina','movement_sprint_speed']]
kmeans.fit(X)
plt.scatter (players['power_stamina'], players['movement_sprint_speed'], c=kmeans.predict(X)) 

````
