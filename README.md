# grantapplication-gis
How to collect and analyze data from grant applications - QGIS project & mockups

The QGIS project consists of various made up point datasets to allow us to make analyses and mockups of the data. 
The GeoPackage contains all the layers and styles excep the basemap which can be added as XYZ tiles from: http://a.basemaps.cartocdn.com/light_all/{z}/{x}/{y}.png

### Different analysis consist of:

####1. The amount of money granted for different areas
Calculate the sum of grants given for certain postal code areas. Then divide the total with grants given for certain forms of art to visualize how the money was divided between artforms.

####2. Hexagon analysis:
create a hexagon grid with hexagons the size of 1km2 & count points in polygon

####3. Calculate the amount of granted applications within a population square (250m2)
count points from the population squares by Stats Finland

####4. Visualize the different themes on map
add the mockup data on map as points, then filter out the unwanted categories & categorize the remaining

####5. The percentage of applied grants per area
Count the amount of points in polygon (the borders of areas from Stats Finland), count the percentage of 'Yes' points from the whole.

####6. Accesibility analysis
Analysis done based with the Catchment plugin by Gispo. The analysis uses the OpenStreetMap database.

The mockup of the map for web browser was done with qgis2web plugin (and a bit of Gimp)
The mockups of the application were made with Adobe Photoshop.
