# US Coronavirus Cases 2020

This project explores the distribution of covid-19 cases in the lower 48 US states from the year 2020. 

## Map 1: US Covid-19 Case Rates
![](img/map1image.JPG)
The [first map](https://sarahg9.github.io/CoronavirusCases2020/map1) is a choropleth map depicting the covid-19 cases per thousand people by each county in the US. Users can hover over individual counties to see the covid rates. The rates are rounded so there is not a fraction of a case of covid. 

## Map 2: US Covid-19 Cases
![](img/map2image.JPG)
The [second map](https://sarahg9.github.io/CoronavirusCases2020/map2) visualizes the total number of covid cases in each county as a proportional symbol map. Users can zoom in and out as well click on the points for each county and see the county name and number of covid cases. 

The maps acts as visualizations of covid case data and these maps can be used to suggest trends in counties and regions and similar maps could be used to inform policy and public health decisions. Primary functions used for making the maps include "map.on" and "geojsonFetch." Both functions, through the inclusion of secondary functions, recongize the data source and then add the data's corresponding layer to the map. 

## Additional Notes
As noted on each map, data was sourced from [The New York Times](https://github.com/nytimes/covid-19-data/blob/43d32dde2f87bd4dafbb7d23f5d9e878124018b8/live/us-counties.csv) while the population data for the rate calculations was from the [US Census Bureau](https://data.census.gov/cedsci/table?g=0100000US%24050000&d=ACS%205-Year%20Estimates%20Data%20Profiles&tid=ACSDP5Y2018.DP05&hidePreview=true). Shapefiles were converted to geojson through [QGIS](https://qgis.org/en/site/). QGIS and its histogram feature were also used to visualize the distribution of cases and inform the decision on the bins for the proportional symbols. [Mapshaper](https://mapshaper.org/) was used to simplify the polygons representing each county. The base code was sourced from [MapBox](https://www.mapbox.com/), the [Lab 3 directions](https://www.mapbox.com/) and the [Lab 4 assignment](https://github.com/jakobzhao/geog495/tree/main/labs/lab04) for GEOG 495. The maps use the Albers projection and were adjusted for between the 25th and 50th parallels. When making the maps, I noticed that even when I set an initial zoom, the zoom changed a little when viewing the maps on a monitor versus a laptop screen. The maps were then designed with the assumption that an audience would likely be viewing the maps on a laptop screen. 