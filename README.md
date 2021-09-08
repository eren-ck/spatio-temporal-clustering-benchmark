# Spatio-Temporal Clustering Benchmark for Collective Animal Behavior

## Abstract

<p align="justify">
Various spatio-temporal clustering methods have been proposed to detect groups of jointly moving objects in space and time. However, such spatio-temporal clustering methods are rarely compared against each other to evaluate their performance in discovering moving clusters. Hence, in this work, we present a spatio-temporal clustering benchmark for the field of collective animal behavior. Our reproducible benchmark proposes synthetic datasets with ground truth and scalable implementations of spatio-temporal clustering methods. The benchmark reveals that temporal extensions of standard clustering algorithms are inherently useful for the scalable detection of moving clusters in collective animal behavior.
</p>

---

### Repository Description

This repository implements various spatio-temporal clustering algorithms and showcases their ability to operate on large amounts of data:

* Built on top of `sklearn`
* Hyperparameter optimization by means of grid search
* Execution time control

### Notebooks and files 

* clustering.ipynb: Performs hyperparameter optimization for clustering algorithms and logs clustering results
* st_clustering.py: Implements ST DBSCAN, ST Agglomerative clustering, ST KMeans, ST OPTICS, ST Spectral Clustering, ST Affinity Propagation, ST BIRCH, ST HDBSCAN
* test_files: Contains small example datasets for testing purposes

### Datasets

The synthetic datasets with ground truth are avaiable here: [[Datasets]](https://doi.org/10.5281/zenodo.5495226)

---

### How to locally run

1. Install Python requirements

```bash
pip install -r requirements.txt
```

2. Open and run the ```clustering.ipynb``` notebook

3. Access the results in the ```cluster_results.log``` log file

---

## License
Released under GNU General Public License v3.0. See the [LICENSE](LICENSE) file for details.
The benchmark was developed at the [Data Analysis and Visualization Group](https://www.vis.uni-konstanz.de/) at the University Konstanz funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) under Germany's Excellence Strategy – EXC 2117 – 422037984.