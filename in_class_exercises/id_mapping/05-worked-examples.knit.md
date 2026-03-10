---
title: "worked Example"
params:
  gse: "GSE233947"
  file_grep: "\\.txt.gz$|\\.tsv.gz$|\\.csv.gz$"
---


# Worked examples with before/after tables

This chapter shows **what the data look like**, **what the IDs look like**, and **how the table changes once mapped**.


``` r
library(knitr)
library(dplyr)
```

```
## 
## Attaching package: 'dplyr'
```

```
## The following objects are masked from 'package:stats':
## 
##     filter, lag
```

```
## The following objects are masked from 'package:base':
## 
##     intersect, setdiff, setequal, union
```

``` r
library(tibble)

kable_head <- function(x, n = 5, caption = NULL) {
  knitr::kable(utils::head(x, n), caption = caption)
}

strip_ensembl_version <- function(x) sub("\\..*$", "", x)
```


## GSE233947

### Raw data preview



















