# data

Place data file(s) in this folder.

Then, include codebooks (variables, and their descriptions) for your data file(s)
using the following format.

## veg_data_rough

Dimensions: 234 obs. of 10 variables. Each row is a species observation. 

- `location`: qualitative character variable; the name of the island the data observation was collected on
- `collected.by`: qualitative character variable; who was taking the observations
- `data`: discrete numerical; date data was recorded
- `gps`: qualitative character variable; plot code as denoted in ArcGIS/GPS unit
- `cover`: discrete ordinal; % cover class for the whole plot (entered as highest number in range) -- not by species
- `height`: discrete ordinal; height classes up to >1.5m, entered as their class code (height range information in metadata, number denotes which class. Height increases as code increases.)
- `common`: qualitative character variable; common name for species observed.
- `spp_code`: qualitative character variable; 6-letter species code
- `spp`: qualitative character variable; scientific name for species observed
- `notes`: qualitative character variable; notes from plot

- ...