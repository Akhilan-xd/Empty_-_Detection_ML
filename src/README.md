# Empty Space Detection
### _To identify the empty space from the workstation to manipulate the objects into the free space without disturbing the environment_
---

**Why K-means?**

- K-means is ideal for segmenting workspace data into clusters, identifying empty vs. occupied regions efficiently. It works with various data types (2D/3D spatial or image data), requires no labeled data, and scales well for large datasets. By clustering and finding centroids, it helps detect free space for object manipulation without disturbing the environment using additional concepts like 'Distance Transforms'.

**What are we trying to do with the Distance Transform?**

- The Distance Transform is used to compute the distance of each pixel (or point) in an environment to the nearest occupied region. Therby, refines the separation of occupied vs free regions by leveraging distance metrics to outline boundaries.

**How are we using K-means and Distance Transform to identify the empty spaces?**

- K-means clusters spatial data to segment occupied vs. free regions, identifying areas of interest. The Distance Transform calculates distances from obstacles, creating a gradient map of free space. Combined, they efficiently detect and quantify empty spaces for safe and strategic object manipulation.

**Also add necessary topics you would like to explain**

- ...

---

### References

[1.] Can be youtube videos

[2.] Papers and Articles

[3.] ...
