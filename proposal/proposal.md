Project proposal
================
Ellie and Finn

``` r
library(tidyverse)
library(broom)
```

## 1. Introduction

In order to better understand the relationship between seabird nesting
sites and plant species and structure, we will use data that Finn
collected from plots on seabird islands in the Gulf of Maine and spatial
data collected by a group of COA students at seabird colonies on those
same islands. Primarily, our project will explore vegetation structure,
species richness, and spatial distribution of vegetation on these colony
islands. We also hope to visualize the relationship between nesting site
choice of different seabird species and plant structure on the islands.
The function of the visualizations we create will primarily be
exploratory, informing further statistical analysis during Finn’s senior
project credits. The question our visualizations will inform: is there a
relationship between the distribution of plant species and the
distribution of nesting seabirds in the Gulf of Maine?

Finn collected the primary dataset for this project on four seabird
islands (Shabby, Great Duck, Heron, Schoodic Islands) during the summer
of 2023. Seabird nesting data was collected in the same year on the same
islands. The island_veg dataset is stored in an excel file.This data
primarily consists of species ids associated with plot codes. Plot codes
are associated with GPS points in ArcGIS. The island_bird dataset
includes species nesting and a GPS point for each nest. Wriley Hodge was
the primary collector of this dataset. The island_veg dataset includes
ordinal, character, and numeric data while the island_bird dataset
includes spatial data associated with character data.

The Gulf of Maine is an important region for sensitive seabird
populations. In the face of rapid climate change, understanding the
ecology of seabird nesting sites may help us develop effective
conservation strategies.

Spatial data – gps points of veg plots and nests Categorical – bird
species, plant species Ordinal – plant height classes, cover classes

## 2. Data

Vegatation data from the seabird islands:

    ## Rows: 234 Columns: 10
    ## ── Column specification ────────────────────────────────────────────────────────
    ## Delimiter: ","
    ## chr (8): location, collected by, date, gps, common, spp_code, spp, notes
    ## dbl (2): cover, height
    ## 
    ## ℹ Use `spec()` to retrieve the full column specification for this data.
    ## ℹ Specify the column types or set `show_col_types = FALSE` to quiet this message.

Seabird nesting data from the islands. We are in the process of getting
this data. The people with access to it are at a conference in Florida.

## 3. Ethics review

## 4. Data analysis plan

During this project, we will take on an untydied dataset collected in
the field. We will tidy the data to make it useful for analysis while
maintaining the integrity of the data. We will also integrate datasets
in order to compare vegetation and bird data. Our primary goal is to
create spatial representations of the vegetation community structure on
each of these islands. We will represent species richness in bar plots
separated by island and ranked by island size. Once we get access to the
island_bird data set, we will overlay eider, black-backed gull, and
herring gull distribution with the vegetation structure from the
island_veg dataset. Hopefully this will give us an idea whether there is
correlation between seabird nests and vegetation structure.
