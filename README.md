# Where Are the Abalone? Suitable Aquaculture Habitat on the U.S. West Coast

## About

This repository contains Homework 3 for EDS 223 (Geospatial Analysis & Remote Sensing) in the UCSB Master of Environmental Data Science program. It identifies which West Coast Exclusive Economic Zones (EEZs) have the most suitable habitat for marine aquaculture, based on sea surface temperature (SST) and depth:

- Averages annual SST from 2008 to 2012 and aligns it with bathymetry data.
- Classifies cells as suitable or unsuitable for oysters (0–70 m depth, 11–30 °C) and maps the total suitable area in each EEZ.
- Wraps the workflow in a reusable function, `map_species_habitat()`, and applies it to abalone.

## Repository Structure

```
eds223-hw3-where-are-the-abalone
├── README.md
├── .gitignore
├── abalone_analysis.qmd      # Quarto document with analysis and maps
├── abalone_analysis.html     # Rendered report
├── abalone_analysis_files/   # Figures generated when rendering
└── data/                     # Not tracked (see Data Access)
    ├── average_annual_sst_2008.tif ... average_annual_sst_2012.tif
    ├── depth.tif
    └── wc_regions_clean.shp (+ .dbf, .prj, .shx)
```

## Data Access

The data is **not stored in this repository** because `data/` is listed in `.gitignore`. To run the analysis, obtain the following datasets and place them in `data/` following the structure shown above:

- **Sea surface temperature:** average annual SST rasters for 2008–2012 from NOAA Coral Reef Watch.
- **Bathymetry:** depth raster from the General Bathymetric Chart of the Oceans (GEBCO).
- **Exclusive Economic Zones:** West Coast EEZ boundaries from Marine Regions.

## Author

Calvin Fu ([@cuvlin](https://github.com/cuvlin))

## References

- NOAA Coral Reef Watch. *Daily Global 5km Satellite Sea Surface Temperature* [Data set].
- GEBCO Compilation Group. *GEBCO Gridded Bathymetry Data* [Data set].
- Flanders Marine Institute. *Marine Regions: Exclusive Economic Zones* [Data set]. https://www.marineregions.org/
- EDS 223 Class Page (found [here](https://eds-223-geospatial.github.io/))

## Acknowledgements

This assignment was completed as part of EDS 223 at the Bren School of Environmental Science & Management, UC Santa Barbara.
