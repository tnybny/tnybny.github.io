---
title: "Learn the K in K-means clustering"
excerpt: "Intelligently split clusters to automatically determine the number of clusters in K-means."
collection: portfolio
---

Basically G-means clustering takes the data and keeps splitting "intelligently" until the subset of data under consideration passes a normality test. <br>
Intelligently here means that the new cluster centers (when one is split) are placed along the direction of maximum variance in the subset of data under consideration at that point in time.

Here's a [video of the progress of G-means clustering algorithm](https://www.youtube.com/watch?v=1aeyQnDk0dA); I recommend playing it at 0.25x speed. And here's [some code](https://github.com/tnybny/G-means) for it.

### Limitations of G-means clustering:
* It makes an assumption that the clusters are normally distributed. Even though this is a common assumption, you cannot use G-means for non-normal clusters.
* In some cases, the data could cause G-means to keep splitting again and again to form tiny clusters. The last two steps in the video show the start of this. This happens because of the way normality tests work.

### If you're interested in reading more:
1. Hamerly, Greg, and Charles Elkan. "Learning the k in K means." Advances in neural information processing systems 16 (2004): 281.
2. Vatsavai, Ranga R., et al. "GX-Means: A model-based divide and merge algorithm for geospatial image clustering." Procedia Computer Science 4 (2011): 186-195.
