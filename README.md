# Clustering_Antarctic_Penguin_Species
Arctic Penguin Exploration: Unraveling Clusters in the Icy Domain with K-means Clustering

## Penguin Clustering: Finding Hidden Groups in Antarctic Penguin Measurements with K-Means | Python, scikit-learn

Applied unsupervised learning to Antarctic penguin measurements with no species labels, to see whether the data splits into natural groups. K-means found 6 clusters, and a table of average measurements shows how each cluster differs.

# CONTEXT
Researchers at Palmer Station had body measurements and sex but no species recorded. They knew at least three species live in the region (Adelie, Chinstrap, Gentoo), so the question was which groups the data itself suggests.

# MY ROLE
I handled preprocessing, choosing the number of clusters, clustering and profiling the groups.

# WHAT I DID
• Inspected the data and one-hot encoded sex into a numeric dummy
• Standardised all five features with StandardScaler so no single unit (grams vs millimetres) dominated the distances
• Ran an elbow analysis (inertia for 1 to 9 clusters) to choose the number of clusters, then chose 6 cluster since it was the elbow location
• Fitted K-means with a fixed random seed and visualised clusters on culmen length vs culmen depth
• Built a profile table (stat_penguins) with the mean of each original measurement per cluster, in the original units

# RESULTS
• 332 penguins grouped into 6 clusters of 29 to 78 birds
• 2 Cluster can be identified with smallest culmen lengths but differ in culmen depth
• The cluster cannot be split by sex

# TECH STACK
Python, pandas, scikit-learn (KMeans, StandardScaler), Matplotlib
