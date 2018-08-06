---
layout: post
date: 2018-7-12 12:08
categories: Research
title: Fox River-Green Bay estuary investigation
tags: Research
---

# Methods

## Sampling sites

_Geogrphical and hydrographic information about sampling locations_


Sampling Date: 2018-07-10

Weather: Sunny

Air temperature: 82/68 F

Humidity: 64%

Wind: Southward, 3.107 mph

Source from: [historic weather](https://www.timeanddate.com/weather/usa/green-bay/historic)


_Map of sampling sites_

<style>
#mapid { height: 600px; }
</style>

<div id="mapid">
<script>
var mymap = L.map('mapid').setView([44.57, -88],11);

var Hydda_Base = L.tileLayer('https://{s}.tile.openstreetmap.se/hydda/base/{z}/{x}/{y}.png', {
	maxZoom: 18,
	attribution: 'Tiles courtesy of <a href="http://openstreetmap.se/" target="blank">OpenStreetMap Sweden</a> &mdash; Map data &copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
}).addTo(mymap);

var myIcon = L.icon({
    iconUrl: 'https://upload.wikimedia.org/wikipedia/commons/thumb/1/11/BlackDot.svg/120px-BlackDot.svg.png',
    iconSize: [20, 20],
    iconAnchor: [10, 10],
    popupAnchor: [-3, -76],
});

var marker12 = L.marker([44.51785,-88.00663333],{icon:myIcon}).addTo(mymap);

var marker13 = L.marker([44.5258522,-88.01033333],{icon:myIcon}).addTo(mymap);

var marker16 =L.marker([44.53593333,-88.00711667],{icon:myIcon}).addTo(mymap);

var marker22 =L.marker([44.55733333,-87.995],{icon:myIcon}).addTo(mymap)

var marker26 = L.marker([44.5955,-87.9995],{icon:myIcon}).addTo(mymap);

var marker32 = L.marker([44.58133333,-87.97966667],{icon:myIcon}).addTo(mymap);

var marker41 =L.marker([44.59633333,-87.95116667],{icon:myIcon}).addTo(mymap)

var marker47 = L.marker([44.6375,-87.95866667],{icon:myIcon}).addTo(mymap);

var marker48 = L.marker([44.6145,-87.90116667],{icon:myIcon}).addTo(mymap);

var marker51 =L.marker([44.65283203,-87.9],{icon:myIcon}).addTo(mymap)

var marker55 = L.marker([44.74166667,-87.88666667],{icon:myIcon}).addTo(mymap);

var marker56 =L.marker([44.71829987,-87.8425],{icon:myIcon}).addTo(mymap)

var marker57 = L.marker([44.69329834,-87.79666667],{icon:myIcon}).addTo(mymap);

var marker1 = L.marker([44.51785,-88.00663333]).addTo(mymap);
marker1.bindPopup("#12").openPopup();

var marker2 =L.marker([44.53593333,-88.00711667]).addTo(mymap);
marker2.bindPopup("#16").openPopup();

var marker3 =L.marker([44.55733333,-87.995]).addTo(mymap)
marker3.bindPopup("#22").openPopup();

var marker4 =L.marker([44.59633333,-87.95116667]).addTo(mymap)
marker4.bindPopup("#41").openPopup();

var marker4 =L.marker([44.65283203,-87.9]).addTo(mymap)
marker4.bindPopup("#51").openPopup();

var marker4 =L.marker([44.71829987,-87.8425]).addTo(mymap)
marker4.bindPopup("#56").openPopup();

</script>
</div>
__
