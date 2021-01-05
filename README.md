# GOES-R NetCDF to Shapefile

These scripts transform GOES-R Series products from their native netCDF format to ESRI shapefiles. Discrete variables, like the Level 2+ Clear Sky Mask product, can
be polygonized easily-- a vector polygon can be created for all connected regions of pixels in the raster sharing a common pixel value. Continous variables,
like Level 2+ Land Suface Temperature, can be transformed into polygons by first segmenting the value range into discrete intervals and then mapping the variable as
a contour plot. 

Determine whether the GOES-R Series product variable-of-interest is discrete or continous, then choose the appropriate script. To use the script, adjust the
satellite, product, date and time, to select a particular image. Adjust the directory to a local path. The script will visualize and download the netCDF file,
and download the resulting shapefile to the local path. 
