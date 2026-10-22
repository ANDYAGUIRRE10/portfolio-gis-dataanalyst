# Urban Heat Island Analysis — Santa Fe, Argentina

**GIS & Data Analytics Portfolio Project | Remote Sensing | Python**

## Overview

This project aims to investigate the spatial distribution of Land Surface Temperature (LST) and vegetation across the urban area of Santa Fe, Argentina, using freely available satellite imagery and open-source geospatial tools.

The analysis will focus on the relationship between surface temperature and vegetation cover, combining remote sensing, raster processing, exploratory data analysis, and thematic cartography.

The project is currently in development.

## Objectives

- Retrieve and process satellite imagery covering Santa Fe, Argentina.
- Estimate Land Surface Temperature (LST) from Landsat 8/9 Level-2 products.
- Calculate the Normalized Difference Vegetation Index (NDVI).
- Explore the spatial relationship between surface temperature and vegetation.
- Generate descriptive statistics, tables, and visualizations using Python.
- Produce thematic maps and communicate the results through GIS outputs.

## Data Sources

- **Landsat 8 and Landsat 9 — Collection 2 Level-2:** surface temperature and surface reflectance products.
- **USGS EarthExplorer:** satellite imagery discovery and download.
- **Supporting geospatial data:** urban boundaries and other reference layers, depending on availability and suitability.

Data selection will consider acquisition dates, cloud cover, spatial coverage, and quality flags.

## Technology Stack

| Technology | Purpose |
|---|---|
| Python | Geospatial processing and analysis automation |
| Rasterio | Raster data access and processing |
| NumPy | Numerical and raster calculations |
| Pandas | Tabular data management and statistical analysis |
| GeoPandas | Vector data processing and spatial analysis |
| Matplotlib | Statistical charts and visualizations |
| QGIS | Thematic cartography and map production |
| Git & GitHub | Version control and project documentation |

## Methodology

The planned workflow consists of the following stages:

1. **Data acquisition:** download suitable Landsat scenes and supporting geographic data.
2. **Quality control:** inspect metadata, cloud masks, valid pixels, and spatial coverage.
3. **Raster processing:** apply the appropriate scale factors and quality masks to satellite bands.
4. **Indicator calculation:** derive LST in degrees Celsius and calculate NDVI from surface reflectance.
5. **Exploratory data analysis:** summarize distributions, calculate descriptive statistics, and examine the relationship between LST and NDVI.
6. **Cartographic production:** create thematic maps in QGIS.
7. **Documentation:** publish the methodology, scripts, selected outputs, and limitations.

## Planned Outputs

- Land Surface Temperature raster and thematic map.
- NDVI raster and vegetation distribution map.
- Descriptive statistics and summary tables in CSV format.
- Statistical charts and visualizations.
- A reproducible Python workflow.
- A QGIS project containing the final cartographic outputs.

## Project Structure

```text
urban-heat-island-santa-fe/
├── README.md
├── environment.yml
├── data/
│   ├── raw/
│   ├── processed/
│   └── reference/
├── notebooks/
├── scripts/
├── qgis/
├── outputs/
│   ├── maps/
│   ├── figures/
│   └── tables/
└── docs/
```

## Analytical Considerations

Land Surface Temperature represents the radiometric temperature of the Earth's surface, not near-surface air temperature.

Landsat thermal data have a coarser native spatial resolution than their standard delivered grid may suggest. Resampling does not create additional independent thermal observations.

The relationship between NDVI and LST will be examined statistically without assuming that correlation alone establishes causation.

Clouds, shadows, acquisition dates, seasonal conditions, and the selection of the study area will be considered when interpreting results.

## Project Status

**In progress — data acquisition and workflow development.**

The analyses, statistical results, and final maps will be added as the project advances.

## Author

**Andrés Aguirre**  
Geographer | GIS & Remote Sensing | Spatial Data Analysis

This project is part of my GIS and Data Analytics portfolio, focused on applying geospatial technologies and reproducible analytical workflows to territorial and environmental questions.
