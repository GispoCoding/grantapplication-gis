# grantapplication-gis
How to collect and analyze data from grant applications - QGIS project & mockups

The aim of the project was to think of the collecing, visualizing and analyzing of the GIS data from grant applications. City of Helsinki recieves plenty of grant applications which contain information about the location of the applicants. How that data could be collected better, visualized on map and analyzed?

At this point all the analysis were done manually, but it is possible to automate the processes. For different ideas about the analysis and the future scenarios, see [our blog post about the projects and its results.](https://gispo.fi/blogi/paikkatietoa-avustushakemuksista/)  

The QGIS project is stored inside the Geopackage file. **The project consists of various made up point datasets to allow us to make analyses and mockups of the data - no official data from the City of Helsinki was given to us nor is available in this repository.**

The GeoPackage contains all the layers and styles except the basemap. The basemap used on the visualizations can be added as XYZ tiles from: http://a.basemaps.cartocdn.com/light_all/{z}/{x}/{y}.png

### Different analysis consist of:

#### 1. The amount of money granted for different areas
Calculate the sum of grants given for certain postal code areas. Then divide the total with grants given for certain forms of art to visualize how the money was divided between artforms.

![image1](/images/Granted-applications-art-sum-types.png)

#### 2. Hexagon analysis:
create a hexagon grid with hexagons the size of 1km2 & count points in polygon (in this case limited to youth work IIRC).

![image2](/images/Granted-applications-as-hexagons.png)

#### 3. Calculate the amount of granted applications within a population square (250m2)
count points from the population squares by Stats Finland

![image3](/images/Granted-applications-per-250m2.png)

#### 4. Visualize the different themes on map
add the mockup data on map as points, then filter out the unwanted categories & categorize the remaining

![image4](/images/Excercise-points.png)

#### 5. The percentage of applied grants per area
Count the amount of points in polygon (the borders of areas from Stats Finland), count the percentage of 'Yes' points from the whole.

![image5](/images/Granted-percentage.png)

#### 6. Accesibility analysis
Analysis done based with the Catchment plugin by Gispo [read more about it here](https://gispo.fi/en/blog/analyzing-school-accessibility-on-qgis/). The analysis uses the OpenStreetMap database.

![image6](/images/Youth-work-accessibility.png)
The accessibility of youth work agents, 15min walk

![image7](/images/Scout-accessibility-15m-walk.png)
The accessibility of scout agents, 15min walk

#### Other mockups

The mockup of the map for web browser was done with qgis2web plugin (and a bit of Gimp)
![image8](/images/Mockup-map-for-browser.jpeg)

The mockups of the application were made with Adobe Photoshop.
![image9](/images/Application-mockup-1.png)
