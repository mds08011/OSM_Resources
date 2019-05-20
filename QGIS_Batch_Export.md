1. Create a folder to store your Shapefiles there (e.g., I've created the folder /tmp/data/, I use GNU/Linux).

2. In QGIS, open the QGIS Python console.

3. Write the following line, editing the right hand side to match the full path to your folder (make sure you include the trailing slash/backslash):
```
myDir = '/tmp/data/'
```
4. Press Enter.

5. Copy the following lines to the QGIS Python console:

```
for vLayer in iface.mapCanvas().layers():
    QgsVectorFileWriter.writeAsVectorFormat( vLayer, 
        myDir + vLayer.name() + ".shp", "utf-8", 
        vLayer.crs(), "ESRI Shapefile" )
```
6. Press Enter a couple of times.
