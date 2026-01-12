# using the bcb420 base image
FROM risserlin/bcb420-base-image:winter2026-arm64

RUN /bin/sh -c R -e 'BiocManager::install(c("DSeq2", "enrichplot"))'

RUN /bin/sh -c install2.r    -d TRUE    -r "https://cran.rstudio.com" pheatmap

