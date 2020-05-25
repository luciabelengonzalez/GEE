# GEE

## Table of contents
* [General info](#general-info)
* [Technologies](#technologies)
* [Scripts](#scripts)


## General info
This repository contains Python scripts that I use to retrieve data from Google Earth Engine platform. 
	
## Technologies
Project is created with:
* Python: 3.6

It is required to install The Earth Engine Python API package:
```

$ pip3 install earthengine-api

```
For more information visit: https://developers.google.com/earth-engine/python_install
	
## Scripts
[retrieve_ndvi_series_s2_by_region](https://github.com/luciabelengonzalez/GEE/blob/master/retrieve_ndvi_series_s2_by_region.ipynb)
Given a FeatureCollection (with a geometry column) with one or more features and a period of time, export 2 csv files with columns "plot", "date" and "NDVI": one with raw data and another with outliers discarded. It is assumed that the region of interest is covered by vegetation. The shapefile must contain an attribute called "layer" with the name of each feature (i.e. plots).

