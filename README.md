# spectral_clustering
The toy example notebook sketches how spectral clustering works on a small perturbed block matrix with three (quasi-)blocks. 

In the real data example the algorithm is applied to real masked data. For this purpose is specified a similarity function, then computed a cluster assignment and reordered similarity matrix according to the identified quasi-blocks.

Once we have identified strongly connected clusters of metrics, we can compute a representative for each cluster by averaging over all assigned metrics. 

Eventually we give an visualization that provides a better insight, which metrics enter into the particular clusters together with a confidence corridor for each represantative.

For real data example we used the scikit-learn implementation of [Spectral Clustering](http://scikit-learn.org/stable/modules/generated/sklearn.cluster.SpectralClustering.html#sklearn.cluster.SpectralClustering) 
