<h3> Richard Dait
<h3> GEOG 458
<h3> 02/12/2021

</br>
</br>
</br>
<h1> <p align="center"> <b> Lab 3: Web Map Application</b> </p>
</br>
<h5> <p align="left"> The purpose of lab 3 is to create an <a href="https://github.com/jakobzhao/geog458/tree/master/labs/lab03" target="_blank">interactive web map</a> with a thematic style that illustrates a chosen statistic or topic. This choropleth map in particular, displays the number of airports within each state, according to pre-defined data intervals. Additionally, symbols are included to represent airports themselves. The standard basemap is from openstreetmap. </p>

<p> L.map and its parameters are assigned to var mymap to hold and build a map. L.tileLayer adds an OpenStreetMap basemap to the screen. boundaries variable is attached to the usstates geoJSON file to delineate U.S. boundaries. Colors variable dynamically builds a color ramp from olorbrewer's oranges using an if/elif/else statements. Airports variable obtains the airports geoJSON file and attaches it to the map. Then, it binds the IATA and displays the city name when an airport is clicked on. An if else statement is used to determine whether or not there is an air traffic tower or not. A legend is added using L.control and a function that runs when it is added to the map. L.control.scale adds a scale to the bottom right as a fundamental cartographic element. A marker applying the click feature is added to represent Seatac.</p>

<h5> <p> For the data source, two geoJSON files were used - airports and usstates. The former was converted from a shapefile, with its original owner being <a href = "https://catalog.data.gov/dataset/usgs-small-scale-dataset-airports-of-the-united-states-201207-shapefile" target = "_blank"> Data.gov</a>. The latter contains state boundaries and was acquired from <a href = "https://bost.ocks.org/mike/" target = "_blank"> Mike Bostock</a>. Plane icon that represent airports is courtesy of Font Awesome. Credit and acknowledge goes towards Professor Bo Zhao and anyone who assisted in designing the lab.</p>
