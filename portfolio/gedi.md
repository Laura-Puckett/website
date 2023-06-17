---
title: "Comparison of Satellite and Airborne LiDAR data"
excerpt: "An exploratory project to compare GEDI and ICESat-2 data against 3DEP discrete-return LiDAR data. <br/><br/><img src='/images/portfolio/gedi_icesat2_als_comparison.png'>"
collection: portfolio
---
In this project, I created a workflow to compare GEDI and ICESat-2 against high-quality discrete-return LiDAR data for an area of interest. The area used for this analysis is a portion of the Sierra Nevada Mountain Range near Lake Tahoe.

- [Code Repository](https://github.com/Laura-Puckett/lidar_comparisons/tree/NAU)

The main steps were to:
1. Download and subset ICESat-2 data for an area of interest
1. Create spatial geometries from ICESat-2 and GEDI data csv files
  - this involved creating different geometries for the two instruments, because they
  have different pulse footprints
1. Extract corresponding discrete-return data for each geometry and calculate
height metrics
1. Intersect geometries with forest group and forest cover layers and calculate summary values for each polygon
1. Visualize the results

**Datasets**

Dubayah, R., Hofton, M., Blair, J., Armston, J., Tang, H., Luthcke, S. (2020). <i>GEDI L2A Elevation and Height Metrics Data Global Footprint Level  V001</i> [Data set]. NASA EOSDIS Land Processes DAAC. Accessed 2020-08-15 from [https://doi.org/10.5067/GEDI/GEDI02_A.001](https://doi.org/10.5067/GEDI/GEDI02_A.001)

Neuenschwander, A. L., K. L. Pitts, B. P. Jelley, J. Robbins, B. Klotz, S. C. Popescu, R. F. Nelson, D. Harding, D. Pederson, and R. Sheridan. 2021. ATLAS/ICESat-2 L3A Land and Vegetation Height, Version 5. [Indicate subset used]. Boulder, Colorado USA. NASA National Snow and Ice Data Center Distributed Active Archive Center. doi: https://doi.org/10.5067/ATLAS/ATL08.005. [2020-08-15].

CA NoCAL Wildfires B1 2018: Discrete-Return LiDAR Data downloaded from [USGS 3DEP LiDAR Explorer](https://prd-tnm.s3.amazonaws.com/LidarExplorer/index.html#/)

B. Ruefenacht, M.V. Finco, M.D. Nelson, R. Czaplewski, <i> et al. <i> (2008). Conterminous U.S. and Alaska Forest Type Mapping Using Forest Inventory and Analysis Data. USDA Forest Service - Forest Inventory and Analysis (FIA) Program & Geospatial Technology and Applications Center (GTAC). Accessed 2020-08-20 from [https://data.fs.usda.gov/geodata/rastergateway/forest_type/](https://data.fs.usda.gov/geodata/rastergateway/forest_type/)
