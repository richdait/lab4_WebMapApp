<h3> Richard Dait
<h3> GEOG 458
<h3> 02/12/2021

</br>
</br>
</br>
<h1> <p align="center"> <b> Lab 3: Web Map Application</b> </p>
</br>
<h4> <b> Introduction</b> </h4> <h5> <p align="left"> The purpose of lab 3 is to create an <a href="https://github.com/jakobzhao/geog458/tree/master/labs/lab03" target="_blank">interactive web map</a> with a thematic style that illustrates a chosen statistic or topic. This choropleth map in particular, displays the number of airports within each state, according to pre-defined data intervals and whether the airport itself, contains an air traffic control tower. The standard basemap is from openstreetmap. </p> </h5>

<h4> <b> Function and Style </b> </h4>
<h5> <p align="left"> An orange graduated color ramp, symbolizes the number of airports per state. California, Texas and Alaska appear to have the most, recording more than 41+. This is illustrated in the darkest orange. Whereas, states such as Oregon and South Dakota have the least - indicated by the lightest of orange. If and else statements were used in a setColor function to classify according to the amount of airports they had. The chroma library scales the groups, with the most intense color equivalent to those states that contain more than 41 airports. As for the two distinct colored plane icons, if else statements within a pointToLayer option, in conjunction with onEachFeature, determines which airport has an air traffic control tower (e.g., if (feature.properties.CNTL_TWR == "Y") {return...}). Black indicates yes, white represents no. 

</p> </h5>

<h4> <b> Acknowledgment, Credits and Data Source </b> </h4>
<h5> <p> For the data source, two geoJSON files were used - airports and usstates. The former was converted from a shapefile, with its original owner being <a href = "https://catalog.data.gov/dataset/usgs-small-scale-dataset-airports-of-the-united-states-201207-shapefile" target = "_blank"> Data.gov</a>. The latter contains state boundaries and was acquired from <a href = "https://bost.ocks.org/mike/" target = "_blank"> Mike Bostock</a>. As for the black and white plane icons that represent airport towers, they are provided by Font Awesome. A big thank you goes towards Professor Bo Zhao and those who assisted in designing the lab.</p> </h5>
