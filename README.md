# My roads

These are the roads I've driven. It starting with an old AAA map I used to mark up with a Sharpie. At first (~2013), I "vectorized" the map using exported KML files from Google Earth for each driving route. Later (2016) I started using the Google Maps API to retrieve JSON directly for those routes. Recently I had to "clean" up the file because overlapping line features had begun to build up in areas where exported routes used the same path. The basic gist of that process was:

1. Clean up any obvious invalid geometries.
2. Buffer line features by 20m
3. Dissolve buffer
4. Create centerlines
5. Simplify line 60m

These routes are updated to the timestamp in the GeoJSON filename. They are simplified to ~60m to reduce file size.
