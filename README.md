The file "ca-water.zip" includes an ESRI Shapefile containing all water areas between 32°N and 43°N, and betweeen 114°W and 125°W. This bounding box contains all of California. 

The water boundaries are derived from [ESRI's World Water Bodies layer](https://www.arcgis.com/home/item.html?id=e750071279bf450cbd510454a80f2e63), cropped to the given latitude/longitude rectangle, and with all features of the same type merged into one feature. To reduce file size, the geometries have been simplified to a precision of 0.0001 geographic degrees, or roughly 36 feet (11 meters).

The file includes two features, one for the Pacific Ocean, and the other for "inland perennial" water bodies (lakes and rivers). This allows the ocean to be distinguished from non-ocean water bodies.
