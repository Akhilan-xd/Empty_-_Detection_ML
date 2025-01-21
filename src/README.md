# Empty Space Detection
### _To identify the empty space from the workstation to manipulate the objects into the free space without disturbing the environment_
---

**Why K-means?**

- K-means is ideal for segmenting workspace data into clusters, identifying empty vs. occupied regions efficiently. It works with various data types (2D/3D spatial or image data), requires no labeled data, and scales well for large datasets. By clustering and finding centroids, it helps detect free space for object manipulation without disturbing the environment using additional concepts like 'Distance Transforms'.

**What are we trying to do with the Distance Transform?**

- The Distance Transform is used to compute the distance of each pixel (or point) in an environment to the nearest occupied region. Therby, refines the separation of occupied vs free regions by leveraging distance metrics to outline boundaries.

**How are we using K-means and Distance Transform to identify the empty spaces?**

- K-means clusters spatial data to segment occupied vs. free regions, identifying areas of interest. The Distance Transform calculates distances from obstacles, creating a gradient map of free space. Combined, they efficiently detect and quantify empty spaces for safe and strategic object manipulation.

**About Silhouette Co-efficient**

- The Silhouette Coefficient is a measure of how well samples are clustered with samples that are similar to themselves. Clustering models with a high Silhouette Coefficient are said to be dense, where samples in the same cluster are similar to each other, and well separated, where samples in different clusters are not very similar to each other.

- The Silhouette Coefficient is calculated using the mean intra-cluster distance (a) and the mean nearest-cluster distance (b) for each sample. The Silhouette Coefficient for a sample is (b - a) / max(a, b). Note that Silhouette Coefficient is only defined if number of labels is 2 <= n_labels <= n_samples - 1.


---

### References

[1.] [Cropping Images](https://learnopencv.com/cropping-an-image-using-opencv/)

[2.] [Image Segmentation with Kmeans](https://www.kaggle.com/code/hal1001k/image-segmentation-with-kmeans)

[3.] [Kmeans - clustering](https://opencv24-python-tutorials.readthedocs.io/en/latest/py_tutorials/py_ml/py_kmeans/py_kmeans_opencv/py_kmeans_opencv.html#kmeans-opencv)

[4.] [Plotting a graph to represent the data](https://www.geeksforgeeks.org/three-dimensional-plotting-in-python-using-matplotlib/)

[5.] [Evaluation Metrics](https://towardsdatascience.com/k-means-clustering-algorithm-applications-evaluation-methods-and-drawbacks-aa03e644b48a)

[6.] [Distance Transform](https://www.geeksforgeeks.org/python-opencv-distancetransform-function/)