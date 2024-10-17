# Implementation-of-K-Means-Clustering-for-Customer-Segmentation

## AIM:
To write a program to implement the K Means Clustering for Customer Segmentation.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the necessary packages using import statement.

2.Read the given csv file using read_csv() method and print the number of contents to be displayed using df.head().

3.Import KMeans and use for loop to cluster the data.

4.Predict the cluster and plot data graphs.

5.Print the outputs and end the program

## Program:
```
/*
Program to implement the K Means Clustering for Customer Segmentation.
Developed by: PRIYADHARSHINI S
RegisterNumber:  212223240129

import pandas as pd
import matplotlib.pyplot as plt
data=pd.read_csv('Mall_customers.csv')
data.head()

data.info()

data.isnull()

data.isnull().sum()

from sklearn.cluster import KMeans
wcss=[]

for i in range(1,11):
    kmeans=KMeans(n_clusters =i,init ="k-means++")
    kmeans.fit(data.iloc[:,3:])
    wcss.append(kmeans.inertia_)


plt.plot(range(1,11),wcss)
plt.xlabel("No. of Clusters")
plt.ylabel("wcss")
plt.title("Elbow Method")

km =KMeans(n_clusters=5)
km.fit(data.iloc[:,3:])

y_pred =km.predict(data.iloc[:,3:])
y_pred

df0.head()

df1.head()

df2.head()

df3.head()

df4.head()

plt.scatter(df0["Annual Income (k$)"],df0["Spending Score (1-100)"],c="red",label="cluster0")
plt.scatter(df1["Annual Income (k$)"],df1["Spending Score (1-100)"],c="blue",label="cluster1")
plt.scatter(df2["Annual Income (k$)"],df2["Spending Score (1-100)"],c="green",label="cluster2")
plt.scatter(df3["Annual Income (k$)"],df3["Spending Score (1-100)"],c="black",label="cluster3")
plt.scatter(df4["Annual Income (k$)"],df4["Spending Score (1-100)"],c="magenta",label="cluster4")
plt.legend()
plt.title("Customer Segments")
*/
```

## Output:
![Screenshot 2024-10-17 141847](https://github.com/user-attachments/assets/abf78096-7812-44e2-a91a-49fde8bbc06a)
![Screenshot 2024-10-17 141856](https://github.com/user-attachments/assets/d086cad3-8bf5-4c3a-b2a7-63b9c9b39464)
![Screenshot 2024-10-17 141904](https://github.com/user-attachments/assets/c915cebe-0ce3-4176-8401-22a04b49e0dd)
![Screenshot 2024-10-17 141922](https://github.com/user-attachments/assets/c2f87d66-4e44-4af6-a5b5-bd8fd24908dc)
![Screenshot 2024-10-17 141932](https://github.com/user-attachments/assets/48574418-c177-4b8b-b771-607ef0acb23e)
![Screenshot 2024-10-17 141942](https://github.com/user-attachments/assets/c23a47cb-f83c-4a80-8804-b7f9872fab81)
![Screenshot 2024-10-17 141948](https://github.com/user-attachments/assets/28f556e0-8718-416f-8fcb-9d01fe65b718)
![Screenshot 2024-10-17 141955](https://github.com/user-attachments/assets/21162449-0fc3-4341-a011-1c2062bff558)
![Screenshot 2024-10-17 142002](https://github.com/user-attachments/assets/25eb3f39-97ce-4e30-a8a5-61cfe57e08dc)
![Screenshot 2024-10-17 142008](https://github.com/user-attachments/assets/45333978-5e4d-4909-9314-b5a5d23bb3c4)
![Screenshot 2024-10-17 142020](https://github.com/user-attachments/assets/6e214a8c-e7e1-4adb-a143-301c6477f169)



## Result:
Thus the program to implement the K Means Clustering for Customer Segmentation is written and verified using python programming.
