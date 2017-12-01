---
layout: post
date: 2017-03-31 14:24
categories: R
title: Learning ggmap
tags: r
---
This is a document for myself to review ggmap package, and how to get quick start.

ggmap is powerful map plot package in R. Compared with maps package, plots exported from ggmaps are elegant.

Two steps to plot a map: plot a map raster, decorate the base map with your own data.

### Step 1: download your base map

You need to know the location you will plot. Define location in two ways showing below:

```
library(ggmap)
Location1 <- "University of Wisconsin, Milwaukee" #Use your address as your defination
Location2 <- "c(lon = -95.3632715, lat = 29.7632836)" # Use longitude and latitude  
```
Use `get_map` function to download the raster map in your location.
There are 3 map “sources” to obtain a map raster, and each of these sources has multiple “map types”
>stamen: “watercolor”, “toner”, "terrain"

![stamen](/image/stamen.jpg)
>googlemap:

![googlemap](/image/googlemap.jpg)
>osm:(sometimes their servers are unavailable)

![osm](/image/osm.jpg)

```
myMap <- get_map(location=myLocation, source="stamen", maptype=“watercolor", crop=FALSE)
ggmap(myMap)
##zoom = integer from 3-21
##3 = continent, 10=city, 21=building
##(openstreetmap limit of 18)
```
### Step 2 deoorate your map with data

---

In addition, a developing R package need to be concerned: [rMap](http://rmaps.github.io/).

### References:
[ggmap github](https://github.com/dkahle/ggmap)

[ggmap document](https://cran.r-project.org/web/packages/ggmap/ggmap.pdf)

[ggmap quick start](https://www.nceas.ucsb.edu/~frazier/RSpatialGuides/ggmap/ggmapCheatsheet.pdf)

[ggmap Introduction](https://dl.dropboxusercontent.com/u/24648660/ggmap useR 2012.pdf)
