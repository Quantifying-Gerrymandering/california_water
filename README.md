# california_water

The file "ca-water.zip" includes an ESRI Shapefile containing all water areas between 32°N and 43°N, and betweeen 114°W and 125°W. This bounding box contains all of California and Nevada, parts of Oregon, Idaho, Utah, and Arizona, and parts of the Mexican states of Baja California and Sonora.

The water boundaries are derived from [ESRI's World Water Bodies layer](https://www.arcgis.com/home/item.html?id=e750071279bf450cbd510454a80f2e63). I opened the layer in ArcGIS Pro. Because the layer is too large to be exported as a shapefile, I cropped it to the aforementioned rectangle before exporting it. Using QGIS, I applied a buffer of 0.0002 degrees to eliminate rounding errors in adjacent oceanic features, and then dissolved contiguous or overlapping features of the same type into a single feature. To further reduce file size, the geometries have been simplified to a precision of 0.0001 degrees, or roughly 36 feet (11 meters). I then exported the geometries as the shapefile "ca-water.zip".

The file includes two features, one for the Pacific Ocean, and the other for "inland perennial" water bodies (lakes and rivers). This allows the ocean to be distinguished from non-ocean water bodies.
