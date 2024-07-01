# Changes in spatial accessibility to primary health care physicians between 2011 and 2022 in Germany (100m Raster)


## Data Description:

This dataset includes a 100 m raster of changes in access to primary care physicians in Germany. It complements the article "Mapping access to medical service provision at micro-scale: Dynamics in supply and demand in Germany", published in the journal *Spatial Research and Planning (https://rur.oekom.de/index.php/rur)*.

For calculating the change in access, data on physicians and population for the years 2011 and 2022 on the level of individual buildings has been combined using the Enhanced Two Step Floating Catchment Area (E2SFCA) method and aggregated into the provided 100 m raster. A maximum travel time of 20 min by car was assumed. 

Physician data consisted of full-time-equivalent (FTE) values for precise physician locations, provided by the *Kassenärztliche Bundesvereinigung (https://www.kbv.de/html/)*. Population for 2011 was taken from the official census and dasymetrically mapped to building footprints, while the data for 2022 has been estimated on building level using an AI-based approach. The calculation of the catchment areas was conducted with *OpenRouteService (https://openrouteservice.org/)*. The aggregation raster is the official INSPIRE 100 m.

The results for the access calculation are presented in a unit we call "Minutes", which can be understood as the theoretical maximum amount of time any person can spend at primary care physicians in a year. The higher the value, the better the access to service provision.


## The attribute table of the raster dataset consists of the FTE, population and access values for the individual years as well as the difference in access between both:

- MEAN_ACCESS_MINUTES_xx: The mean calculated access value for all population locations within a cell in Minutes for the indicated year.
- POPULATION_xx: The population value for this cell. 2011 is the official census value, 2022 is estimated on building level and summarized within a cell.
- FTE_xx: The sum of all physician full-time-equivalents within a cell.
- DIFF_ACCESS_MINUTES: The difference in access between 2011 and 2022, in Minutes.


# Basic information:
- Format: GeoJSON
- Resolution: 100 x 100 m
- Coordinate System: EPSG: 3035 (ETRS89, LAEA)
- Reference year: 2022
- Coverage: Germany


# For details on data access, quality, method and use restriction, please directly consult with [Mr. Reiter](https://www.ioer.de/institut/beschaeftigte/reiter)


# Cite as:
Reiter, D., Jehling, M., & Hecht, R. (2024). Changes in spatial accessibility to primary health care physicians between 2011 and 2022 in Germany (100m Raster) (Version 1.0) [Data set]. Leibniz Institute of Ecological Urban and Regional Development. https://doi.org/10.26084/IOERFDZ-DATA-DE-2024-6


#Note:

This is an early release; the identical dataset will be accessible via ioer-fdz data repository soon along with download services.


**Acknowledgement:** This research is part of the project "GOAT 3.0" which is financed by mFUND (FKZ: 19F2202C).
