# Barbados in QGIS: Adding Vectors and Layers
[originally used on Monday March 28, 2016]
![Test image](/images/BarbadosFlag.png)
### This tutorial is designed so you can practice the skills you used in the [Programming Historian QGIS Tutorial about adding layers](http://programminghistorian.org/lessons/qgis-layers "Links to Programming Historian")
1.	Make a folder or directory called “Barbados” on your computer.
2.	Download the following Barbados data sets from DIVA-GIS [Google it] into that directory and unzip them; each should be in its own sub-directory.
    -	Administrative Areas BRB\_adm.ZIP
    -	Roads BRB\_rds.ZIP
3. 	Open QGIS and set up up a new project.
4.	Set up CRS (Coordinate Reference System) so that the project is using the Barbados 1938 Geographic Coordinate system.

***We need an image here,a screenshot from QGIS showing how to choose the CRS***

![Placeholder image](/images/Barbados1.jpg)
5.	Build a base map: Open these vectors, then change the way they look using the “properties”
    - BRB\_adm0.shp; change so there is no color fill. Remember “fill style” = “no brush”
    - BRB\_adm1.shp; same as above
    - BRB\_roads.shp; change the color and width of the lines so they are easier to see

***We need an image here, another screenshot from QGIS showing what the result should look like***
![Placeholder image 2](/images/Barbados_map.jpg)
6.	Look at the attribute table of BRB\_adm1.shp. These show the country’s 10 parishes. Note which one of the columns gives the name of the parish. Write down the name of that column. Close the attribute table. Go into the “properties” for BRB\_adm1.shp into “labels”. Change so that your map shows the names of the parishes in a large font.
7.	Go to Blackboard and from the Barbados tutorial area, download the file named Dominia-angolorum-BarbadosTIF.zip. Unzip it and import the .tif file into QGIS as a raster file. Note: I have already geo-referenced this file.
8.	Go back to BRB\_adm0.shp and BRB\_adm1.shp and change the width of the lines so they are visible.
9.	In the left-hand “layers” panel, drag the Dominia-angolorum … layer so you can see the parish lines over the historical map.

*** We could use another screenshot here***

![Placeholder image 3](/images/barbadosMMG.jpg)
10.	Go back to Blackboard and download the file named Thompson\_Barbados_1817.tif. Import that into QGIS. [Note: I have already geo-referenced this file.]
11.	Save your work. Close QGIS

# Data Sources for this Tutorial
## Country GIS base map data
http://www.diva-gis.org/gdata

## Historical maps
The map "Dominia anglorum in præcipuis insulis Americæ ut sunt insula" can be downloaded aat https://www.loc.gov/item/74690902/

Other sites that are likely to have similar maps are:
* http://DavidRumsey.com
* [The John Carter Brown Library Map Collection](https://www.brown.edu/academics/libraries/john-carter-brown/jcb-online/image-collections/map-collection)
