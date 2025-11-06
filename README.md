# FeatPairs

**FeatPairs** is an R package for robust feature pair analysis of count data, initially applied to microbiome sequencing counts to derive a "patient discrimination index" (PDI) for early-stage lung cancer prediction (Gut Microbes, 2020, DOI: [10.1080/19490976.2020.1737487](https://doi.org/10.1080/19490976.2020.1737487)) and further extended to feature-module pair ratios for noisy single-cell RNA-seq data and successfully applied in colon cancer cell (CRC) drug-resistant transidifferentiation analysis (Cancer Cell, 2025, Accepted). It also includes UMAP dimension reduction and SNN network building for integration with Seurat and Python packages like Scanpy.

## Installation
Download FeatPairs_1.0.0.tar.gz and install it in R:
```R
install.packages("FeatPairs_1.0.0.tar.gz")
```

## CRC organoid drug-resistance scRNA-seq dataset (in collaboration with Yijun Gao lab)
The single cell dataset is derived from KRAS-mutant colon cancer patient-derived organoids evolved under the pressure of dual inhibitors. This dataset is now released publicly (https://ngdc.cncb.ac.cn/omix/release/OMIX011372).

## Run FeatPairs analysis on the CRC dataset
The parameters for replication of this study are:   
```R
FeatModPairs(counts=counts, logcounts=NULL, n.ctrl.feats=300, n.ctrl.mods=50, n.ctrl.nn=30, minsize.ctrl.mod=3, n.var.feats=2000, span=0.3, pca=T, pca.scale=T, adjust.modcount=F, adjust.dist.scale=F, use.snn=F, impute.ctrl.feats=F, impute.ctrl.mods=F, pca.dim1=1, pca.ndim=25, seed.pca=8888, seed.umap=8888)
```
