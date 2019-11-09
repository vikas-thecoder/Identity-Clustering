# Identity-Clustering
This is my mini project
 In this there are two module first encoding amd second clustering.
 1.First download this modules and stores this modules in cluster folder in your local device.
 3.Now ceate the dataset folder which contain all the images which you want cluster.Place this also in the cluster folder.
 3.Then run encoding module to create a pickle file which contain the encoding of all the images in the dataset.
 4.Now run the cluster module which create the cluster dataset folder and place all the cluster data in the different folder and also        unknown in unknown folder.
 
 NOTE:- In this you can use either a Convolutional Neural Network (CNN) or Histogram of Oriented Gradients (HOG) method to detect the faces in an input image prior to quantifying the face. The CNN method is more accurate (but slower) whereas the HOG method is faster (but less accurate).
 
CLUSTERING FACESs:
 
Now that we have quantified and encoded all faces in our dataset as 128-d vectors, the next step is to cluster them into groups.

Our hope is that each unique individual person will have their own separate cluster.

The problem is, many clustering algorithms such as k-means and Hierarchical Agglomerative Clustering, require us to specify the number of clusters we seek ahead of time.

For this example we know there are only five soccer players — but in real-world applications you would likely have no idea how many unique individuals there are in a dataset.

Therefore, we need to use a density-based or graph-based clustering algorithm that can not only cluster the data points but can also determine the number of clusters as well based on the density of the data.

For face clustering I would recommend two algorithms:

Density-based spatial clustering of applications with noise (DBSCAN)
Chinese whispers clustering
We’ll be using DBSCAN for this tutorial as our dataset is relatively small. For truly massive datasets you should consider using the Chinese whispers algorithm as it’s linear in time.

The DBSCAN algorithm works by grouping points together that are closely packed in an N-dimensional space. Points that lie close together will be grouped together in a single cluster.

DBSCAN also naturally handles outliers, marking them as such if they fall in low-density regions where their “nearest neighbors” are far away.


Special Credit to adrian sir for guiding me in this project.There work are useful for developing this project.
