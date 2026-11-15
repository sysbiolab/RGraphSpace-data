# RGraphSpace-data

Demonstration datasets for the
[RGraphSpace](https://github.com/sysbiolab/RGraphSpace) package vignettes.

The files are published as release assets, not committed to the repository.

## Datasets

| File | Release | Contents | Used in |
|---|---|---|---|
| `gs_spatial_roi.RData` | [v1](https://github.com/sysbiolab/RGraphSpace-data/releases/tag/v1) | `spe_roi` (*SpatialExperiment*) and `gs_roi` (*GraphSpace*): a region of interest of a Visium HD colorectal cancer section, with cell outlines | Spatial-segmented data vignette; downstream analysis vignette |

## Usage

```r
url <- paste0("https://github.com/sysbiolab/RGraphSpace-data/releases/download/",
  "v1/gs_spatial_roi.RData")
f <- tempfile(fileext = ".RData")
download.file(url, f, mode = "wb")
load(f)   # loads 'spe_roi' and 'gs_roi'
```

## Source and terms

The `gs_spatial_roi.RData` file is derived from the 10x Genomics Visium HD human
colorectal cancer dataset (Oliveira et al., 2025), retrieved via
[OSTA](https://bioconductor.org/books/release/OSTA/). It is distributed under
the same terms as the original data.
