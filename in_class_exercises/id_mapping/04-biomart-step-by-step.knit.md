---
title: "Biomart step by step"
params:
  ensembl_version: 115
---

# biomaRt step-by-step

This follows the following workflow: **choose a mart → choose a dataset → discover filters/attributes → query with getBM() → merge back into your matrix**.


``` r
library(biomaRt)
```


## 1. List marts


``` r
listMarts()
```

```
##                biomart                version
## 1 ENSEMBL_MART_ENSEMBL      Ensembl Genes 115
## 2   ENSEMBL_MART_MOUSE      Mouse strains 115
## 3     ENSEMBL_MART_SNP  Ensembl Variation 115
## 4 ENSEMBL_MART_FUNCGEN Ensembl Regulation 115
```

## 2. (Optional) pin an Ensembl archive version



















