# LA Metro

## Commands After Cloning Repository

$ cd /Users/Shawn/Documents/GitHub/la-metro

$ cd. > index.html

$ git add index.html

$ git commit -m “Add index.html”

**input starter code**

$ git add index.html

$ git commit -m “Focus basemap”

$ mkdir data

**LA County shapefile from:**
*https://hub.arcgis.com/datasets/lacounty::la-county-city-boundaries/*

**LA Metro shapefiles from:**
*https://developer.metro.net/docs/gis-data/overview/*

$ git add data/

$ git commit -m “Add data”

$ cd data/Rail_Stations

$ ogr2ogr Stations_All_0715_4326.shp -t_srs "EPSG:4326" Stations_All_0715.shp

$ ogr2ogr -f "GeoJSON" ../rail_stations.json Stations_All_0715_4326.shp

**repeat for other shapefiles in respective folders**

**finish up index.html**

$ git add index.html

$ git commit -m “Finish index.html”

$ git push origin master
