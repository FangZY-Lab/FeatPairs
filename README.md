# FeatPairs

**FeatPairs** is an R package for robust feature pair analysis of count data, initially applied to microbiome sequencing counts to derive a "patient discrimination index" (PDI) for early-stage lung cancer prediction (Gut Microbes, 2020, DOI: [10.1080/19490976.2020.1737487](https://doi.org/10.1080/19490976.2020.1737487)). This implementation extends to feature-module pair ratios, suitable for noisy single-cell RNA-seq data. It includes UMAP dimension reduction and SNN network building for integration with Seurat and Python packages like Scanpy.

## Installation
```R
devtools::install_github("YourGitHubUsername/FeatPairs")
