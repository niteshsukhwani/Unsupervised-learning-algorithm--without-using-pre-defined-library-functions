# Unsupervised-learning-algorithm--without-using-pre-defined-library-functions
## Clustering
1. Cluster: a collection of data objects
<br/>1.1. Similar to one another within the same cluster
<br/>1.2. Dissimilar to the objects in other clusters
2. Clustering is a technique for finding groups of objects such that the objects in a group will be similar (or related) to one another and different from (or unrelated to) the objects in other groups
3. Clustering is often called an unsupervised learning task as no class values denoting an a priori grouping of the data instances are given, which is the case in supervised learning. 
## Examples of Clustering Applications
1. Marketing: Help marketers discover distinct groups in their customer bases, and then use this knowledge to develop targeted marketing programs
2. Land use: Identification of areas of similar land use in an earth observation database
3. Insurance: Identifying groups of motor insurance policy holders with a high average claim cost
4. City-planning: Identifying groups of houses according to their house type, value, and geographical location
5. Earth-quake studies: Observed earth quake epicenters should be clustered along continent faults
## Major Clustering Approaches
1. Partitioning algorithms: Construct various partitions and then evaluate them by some criterion
2. Hierarchy algorithms: Create a hierarchical decomposition of the set of data (or objects) using some criterion
3. Density-based: A cluster is defined as a maximal set of density connected points
4. Grid-based: These algorithms partition the data space into a finite number of cells to form a grid structure and then form clusters from the cells in the grid structure. Clusters correspond to regions that are more dense in data points than their surroundings
## K-means  algorithm
Given the cluster number K, the K-means  algorithm is carried out in three steps after initialization:
<br/>Initialization: set seed points (randomly)
1. Assign each object to the cluster of the nearest seed point measured with a specific distance metric
2. Compute new seed points as the centroids of the clusters of the current partition (the centroid is the centre, i.e., mean point, of the cluster)
3. Go back to Step 1), stop when no more new assignment (i.e., membership in each cluster no longer changes)

## K-Medoids Clustering 
1. Pick a number, k, of random data items as medoids
2. Calculate ARGMIN(TCmn)
3. If TCmn < 0, replace m by n and go back to 2
4. Assign every item to its nearest medoid
## CLARA (Clustering Large Applications) 
1. Draw multiple samples of the data set
2. Apply PAM to each sample 
3. Return the best clustering
## UPGMA: Un-weighted Pair-Group Method Average.

### Merge Strategy:
1. Average-link approach
2. The distance between two clusters is measured by the average distance between two objects belonging to different clusters

## DBSCAN
1. Clustering based on local connectivity and density functions
2. Basic idea 
<br/>2.1. Clusters are dense regions in the data space, separated by regions of lower object density
<br/>2.2. A cluster is defined as a maximal set of density connected points
<br/>2.3. Each cluster has a considerable higher density of points than outside of the cluster
3. Major features:
<br/>3.1. Discover clusters of arbitrary shape
<br/>3.2. Handle noise
<br/>3.3. One scan

