# FeatPairs

**FeatPairs** is an R package for robust feature pair analysis of count data, initially applied to microbiome sequencing counts to derive a "patient discrimination index" (PDI) for early-stage lung cancer prediction (Gut Microbes, 2020, DOI: [10.1080/19490976.2020.1737487](https://doi.org/10.1080/19490976.2020.1737487)). This implementation extends to feature-module pair ratios, suitable for noisy single-cell RNA-seq data. It includes UMAP dimension reduction and SNN network building for integration with Seurat and Python packages like Scanpy.

## Installation
Download FeatPairs_1.0.0.tar.gz and install it in R:
```R
install.packages("FeatPairs_1.0.0.tar.gz")
```

## Application to a CRC organoid scRNA-seq dataset
In a collaborative study with Yijun Gao lab, we have applied this method to a single cell dataset from KRAS-mutant colon cancer patient-derived organoids evolved under the pressure of dual inhibitors. 
This dataset will be released publicly for testing after publication of the study (Zhang et. al. under review).
The parameters used for this study are: n.ctrl.feats = 300, n.ctrl.mods = 50, n.ctrl.nn = 30, minsize.ctrl.mod = 3, n.var.feats = 2000, span = 0.3, pca = T, pca.scale = T, adjust.modcount = F, adjust.dist.scale = F, use.snn = F, impute.ctrl.feats = F, impute.ctrl.mods = F, pca.dim1 = 1, pca.ndim = 25, seed.pca = 8888, seed.umap = 8888.
