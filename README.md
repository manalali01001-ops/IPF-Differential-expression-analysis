# GSE150910 — Idiopathic Pulmonary Fibrosis

## Overview

Python-based differential expression analysis of gene-level count data from **GSE150910**, comparing control and idiopathic pulmonary fibrosis (IPF) samples.

## Workflow

* Data loading and preprocessing
* CPM normalization
* Low-expression gene filtering
* Kolmogorov-Smirnov (KS) differential expression testing
* Log2 fold-change calculation
* Bonferroni correction
* DEG identification
* Hierarchical clustering and gene correlation analysis

## Results

* **Samples:** 206 (103 control, 103 IPF)
* **Genes before filtering:** 18,838
* **Genes after filtering:** 11,097
* **Significant DEGs:** 79
* **Upregulated:** 65
* **Downregulated:** 14

DEGs were defined as:

```text
Adjusted p-value ≤ 0.05
|log2 fold change| ≥ 2
```

## Tools

Python, NumPy, SciPy, Matplotlib, Seaborn, fastcluster

## Data

**GEO:** GSE150910
https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE150910

This project demonstrates a Python-based transcriptomic analysis workflow from raw gene-level counts to differential expression results and visualization.
