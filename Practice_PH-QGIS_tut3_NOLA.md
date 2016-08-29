# New Orleans in QGIS: Creating New Vector Data from Historical Maps
[originally used Monday April 4, 2016]
### This tutorial is designed to reinforce the skills you learned in [Programming Historian QGIS Tutorial\#3](http://programminghistorian.org/lessons/vector-layers-qgis "Links to Programming Historian")

1. Download the NOLA zipfile from Blackboard and unzip it to a folder on your computer.
2. Start a new project; set the CRS: type 26982 to bring up NAD83/ Louisiana south
3. Add Vector: Load the NaturalEarth [ne] shapefile basemap for Louisiana: ne_Louisiana\_10m_admin\_1.shp; Turn the fill color off
4. Add Vector: Load the Open Street Map [OSM] shapemap basemaps for New Orleans – go in this order and look at each. As you look for the files, notice the size of each of them. [Which file is the largest? Which is the smallest? Why?] Once they load, use the right-click “Zoom to Layer” feature and then the magnifying glass. Drag them into the stack-order that makes the most sense to you.
   - OSM\_NOLA\_land\_coast_polygons.shp
   - OSM\_NOLA\_admin\_any.shp
   - OSM\_NOLA\_waterareas\_any.shp
   - OSM\_NOLA\_roads\_any.shp
   - OSM\_NOLA\_buildings\_any.shp
5. Turn labels on for the roads layer so you can see the names of the roads
6. Turn the buildings layer off to make the map easier to view 
7. Add Raster: Load the 1854 Norman Map [this is actually a late 1800s re-creation]. Note: I have already georeferenced this file. Notice the discrepancies in the georeferencing between the historical map and the OSM basemaps. Where are they? 
8. Add Raster: Load the page from 1883 Robinson Atlas of New Orleans. Note: I have already georeferenced this file.
9. Create a point shapefile called “points\_interest’. In that file you will use points to locate buildings you think have disappeared.  [HINT: for more convenient viewing, download the Norman and Robinson maps from Blackboard and view them in a separate image viewer]
10. Build an attribute table for these points, with these attributes
    * Name
    * Year [will be the same as the map]
11. Edit the new shapefile
    * Add 4 points from the 1854 Norman Map
    * Add 2 points from the 1883 Robinson Atlas page
    * Change “properties” to display the new name and date info
12. Create a line shapefile for roads and an attribute table with these fields
    * Name
    * Year
13. Trace 4 roads from the Norman map and them to compare to modern roads
14. Create a new polygon shapefile with "building_name" and "year" attributes
    * Trace 2 buildings as polygons, assisted by the 'snapping' function
15. Save the whole project as a “NOLA.qgs” file so you can load it later.
16. Zoom in on downtown New Orleans with a view that shows your new vector files but NOT the historical maps.
17. Open Print Composer; then Layout, then Add Map to show this downtown area. Leave enough space at the top or bottom of the page for your title
18. Go back to the main screen of QGIS, Zoom out to show the full extent of Louisiana. Turn off the buildings and roads areas [to speed up loading]
19. Then back in Print Composer, add an insert map [Layout/Add Map] that shows the whole state.
    * Put frames around both Map0 and Map1
    * Add a scalebar in Map0, with units in feet [Layout/Add Scalebar]
    * Add a Title to the map [Layout/AddLabel] and add another smaller label identifying the sources of the data.
20. Save the printer composer file and then export a PDF[Composer/Export as PDF]. Put your last name in the PDF filename and upload it to Blackboard

# Data sources for this tutorial:
1. Base map of Louisiana/Texas, etc. from http://NaturalEarthData.com [cultural vectors]; 
2. Base map showing many specific features of New Orleans https://data.nola.gov/
3. Detailed base map of city and surrounding area; http://www.Mapzen.com -- features metro extracts of OpenStreetMap [OSM]
4. Benjamin Norman, _Norman's Plan of New Orleans & Environs_ [New Orleans?, 1854]. https://www.loc.gov/item/2012593335/
5. Elisha Robinson, _Atlas of the Citiy of New Orleans, Louisiana, based upon surveys furnished by John F. Braun_. New York: E. Robinson, 1883. http://www.orleanscivilclerk.com/robinson/guide.htm
