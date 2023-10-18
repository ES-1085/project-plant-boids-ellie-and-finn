Proposal data
================
Ellie and Finn

``` r
library(tidyverse)
library(broom)
```

``` r
data.rough <- read.csv("veg_data_rough.csv")
```

## veg_data_rough

``` r
head(data.rough
     )
```

    ##   location collected.by      date     gps cover height          common spp_code
    ## 1    heron         finn 5/27/2023 hrn3114     1      1            <NA>     <NA>
    ## 2    heron         finn 5/27/2023 hrn2936     1      1            <NA>     <NA>
    ## 3    heron         finn 5/27/2023 hrn3058   100      2        valerian  val off
    ## 4    heron         finn 5/27/2023 hrn3058   100      2       dandelion  tar off
    ## 5    heron         finn 5/27/2023 hrn3058   100      2 stinging nettle  urt dio
    ## 6    heron         finn 5/27/2023 hrn3058   100      2      strawberry  fra vir
    ##                     spp
    ## 1                  <NA>
    ## 2                  <NA>
    ## 3 Valeriana officinalis
    ## 4  taraxacum officinale
    ## 5         urtica dioica
    ## 6   fragaria virginiana
    ##                                                                                                       notes
    ## 1                                                                     trans 4 -> HERG nest ~3m out of range
    ## 2 1) HERG nest w/ 3 eggs just out of range, 2) HERG w/ 2 1m off, 1 w/in radius (don't want to double count)
    ## 3                                                                                                          
    ## 4                                                                     (drawing on datasheet of leaf margin)
    ## 5                                                                                                          
    ## 6

- `location`: qualitative character variable; the name of the island the
  data observation was collected on
- `collected.by`: qualitative character variable; who was taking the
  observations
- `data`: discrete numerical; date data was recorded
- `gps`: qualitative character variable; plot code as denoted in
  ArcGIS/GPS unit
- `cover`: discrete ordinal; % cover classes (entered as highest number
  in range)
- `height`: discrete ordinal; height classes up to \>1.5m, entered as
  their class code (height range information in metadata, number denotes
  which class. Height increases as code increases.)
- `common`: qualitative character variable; common name for species
  observed.
- `spp_code`: qualitative character variable; 6-letter species code
- `spp`: qualitative character variable; scientific name for species
  observed
- `notes`: qualitative character variable; notes from plot

Each row is a species observation. - …
