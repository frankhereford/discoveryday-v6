# discoveryday-v6
## Learn how to use pgrouting for network analysis

### Data
* https://download.geofabrik.de/north-america.html
  * Using subset of OSM clipped to TX

### Tools
* https://github.com/pgRouting/docker-pgrouting
* https://github.com/pgrouting/osm2pgrouting
* QGIS

### Commands that have been helpful

##### Strip out tags from data and convert out of the PBF format
`osmconvert ./texas-latest.osm.pbf --drop-author --drop-version --out-osm -o=texas.osm`

##### Import OSM file
`osm2pgrouting --f ./texas.osm --conf mapconfig.xml --dbname texas --username frank --password atxroutes texas --clean`