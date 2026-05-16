# Implementation-of-K-Means-Clustering-for-Customer-Segmentation

## AIM:
To write a program to implement the K Means Clustering for Customer Segmentation.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the required libraries such as NumPy, Pandas, Matplotlib, and Scikit-learn.

2.Load the customer dataset and select the required features for clustering.

3.Use the Elbow Method to determine the optimal number of clusters.

4.Apply the K-Means clustering algorithm to group the customers into clusters.

5.Visualize the clusters using a scatter plot.

6.Display the cluster centroids and segmented customer groups.
## Program:
```
/*
Program to implement the K Means Clustering for Customer Segmentation.
Developed by: VIGNESH.K
RegisterNumber:  212225240183
import pandas as pd
import matplotlib.pyplot as plt
from sklearn.cluster import KMeans

data = pd.read_csv("Mall_Customer.csv")

X = data.iloc[:, [3, 4]].values

kmeans = KMeans(n_clusters=5, random_state=0)

y_kmeans = kmeans.fit_predict(X)

plt.scatter(X[:, 0], X[:, 1], c=y_kmeans, s=50)

 
plt.scatter(kmeans.cluster_centers_[:, 0],
            kmeans.cluster_centers_[:, 1],
            s=200,
            marker='X')

plt.xlabel("Annual Income")
plt.ylabel("Spending Score")
plt.title("Customer Segmentation using K-Means")

plt.show()
*/
```

## Output:
<img width="1251" height="752" alt="image" src="https://github.com/user-attachments/assets/e312b80e-f542-4d74-a3c9-566b65aeba79" />



## Result:
Thus the program to implement the K Means Clustering for Customer Segmentation is written and verified using python programming.
