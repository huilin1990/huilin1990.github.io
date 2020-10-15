---
layout: post
date: 2017-9-28 17:12
categories: Research
title: Milwaukee River Sampling Protocol
tags: Research
---

# Methods

## Sampling sites

Milwaukee River provides significant nutrient supplies for Lake Michigan. According to (Fillingham 2015), the average daily flux of phosphrus asa approximately 250 kg d<sup>-1</sup>. Three locations, representing the Upstream, Downstream, and mixing Estuary, were selected as water sampling sites (Figures below). *In situ* specific conductivity, distance to Milwaukee Downtown area, and were considered during sampling sites selection. Water temperature, specific conductivity were measured during sampling.

_Geogrphical and hydrographic information about sampling locations_
<iframe width="800" height="250" frameborder="0" scrolling="no" src="//plot.ly/~a54144/18.embed"></iframe>

_Map of sampling sites_
 <link rel="stylesheet" href="https://unpkg.com/leaflet@1.7.1/dist/leaflet.css"
   integrity="sha512-xodZBNTC5n17Xt2atTPuE1HxjVMSvLVW9ocqUKLsCC5CXdbqCmblAshOMAS6/keqq/sMZMZ19scR4PsZChSR7A=="
   crossorigin=""/>
   
   <script src="https://unpkg.com/leaflet@1.7.1/dist/leaflet.js"
   integrity="sha512-XQoYMqMTK8LvdxXYG3nZ448hOEQiglfqkJs1NOQV44cWnUrBc8PkAOcXy20w0vlaXaVUearIOBhiXZ5V3ynxwA=="
   crossorigin=""></script>
   
<style>
#mapid { height: 600px; }
</style>

<div id="mapid">
<script>
var mymap = L.map('mapid').setView([43.07, -87.92],12);

L.tileLayer('https://api.mapbox.com/styles/v1/{id}/tiles/{z}/{x}/{y}?access_token={accessToken}', {
    attribution: 'Map data &copy; <a href="https://www.openstreetmap.org/">OpenStreetMap</a> contributors, <a href="https://creativecommons.org/licenses/by-sa/2.0/">CC-BY-SA</a>, Imagery © <a href="https://www.mapbox.com/">Mapbox</a>',
    maxZoom: 18,
    id: 'mapbox/streets-v11',
    tileSize: 512,
    zoomOffset: -1,
    accessToken: 'pk.eyJ1IjoiYTU0MTQ0IiwiYSI6ImNrZ2I5NmExczBleTAycnRoMTBveGFvazAifQ.M2spDVYVzk3GOr1yY-5Zdw'
}).addTo(mymap);

var marker1 = L.marker([43.025392,-87.903591]).addTo(mymap);
marker1.bindPopup("<b>Estuary</br></b>Milwaukee County Boat Launch").openPopup();

var marker2 =L.marker([43.133424, -87.928420]).addTo(mymap)
marker2.bindPopup("<b>Upstream</b><br>Kletzsch Park.").openPopup();

var marker3 =L.marker([43.0489, -87.8906]).addTo(mymap)
marker3.bindPopup("<b>Euphotic Lake</b><br>Veterans Park.").openPopup();

var marker4 =L.marker([43.03529, -87.9101532]).addTo(mymap)
marker4.bindPopup("<b>Downstream</b><br>Milwaukee Public Market.").openPopup();

</script>
</div>
__

## Stirred Cell Ultrafiltration

Colloids larger than 1 kDa in water samples werer concentrated using Amicon stirred cell ultrafiltration. 180 ml water samples were poured into the cell.

### Ultrafiltration Permeation Model

## Calibration

### Time Calibration

Fractionated colloids flowed through 2-channel UV detectors and two 2-channel fluorescence detectors in sequence. The delay times of each detectors were determined using quinine sulfate solution. Absorption at 254 nm were determined using the UV-Visable spectrophotometer online detector. Excitation/emission wavelength for four channels were set to 310/450 nm. The table below shows average delay time of each detectors against the first UV channel 1.

<iframe width="700" height="300" frameborder="0" scrolling="no" src="//plot.ly/~a54144/14.embed"></iframe>

### Online fluorescence detectors Calibration

A concentration series of quinine sulfate solution, including 2 ppb, 5 ppb, 10 ppb, 20 ppb, 50 ppb, were used for fluorescence calibration.
According to (Eaton, 1988), the fluorescence maximum was measured at 310/450 nm.

<iframe width="900" height="600" frameborder="0" scrolling="no" src="//plot.ly/~a54144/13.embed"></iframe>

Therefore, Excitation/emission wavelength in four detectors were set to 310/450 nm. Quinine sulfate was injected directly without flow through the FlFFF channel. a platform was observed after each injection. The mean values of the platform indicates the concentration of quinine sulfate.

<iframe width="900" height="600" frameborder="0" scrolling="no" src="//plot.ly/~a54144/4.embed"></iframe>

Calibration curves were constructed for four fluorescence detectors (Figure and table below).

<iframe width="900" height = "600" frameborder="0" scrolling="no" src="//plot.ly/~a54144/8.embed"></iframe>
<iframe width="800" frameborder="0" scrolling="no" src="//plot.ly/~a54144/10.embed"></iframe>


## Size-fractionated colloids excitation-emission matrix

Online fluorescence detectors targeted on sixteen excitation-emission wavelengths in the area between the first order Ramen and Rayleigh scatter peak and the second order Ramen and Rayleigh scatter peak. Injections of ultrafiltrated water samples were repeated four times. Between sample injections, excitation-emission wavelengths in fluorescence detectors were altered.  

### DOM from eutrophic lake (Animation below).

Dissolved organic matter from eutrophic lakes contains more autochthonous dissolved organic matter. It was collected in Oct 05, 2017.

<iframe src="https://giphy.com/embed/3ov9jHWCrPGLeVD7TW" width="480" height="359" frameBorder="0" class="giphy-embed" allowFullScreen></iframe>

### DOM from Milwaukee River upstream.

Terresgenious dissolved organic matter might be the dominated component in the composition of DOM in upstream Milwaukee River water.

<iframe src="https://giphy.com/embed/3ohnEnLLGSDFfQ7Y0E" width="480" height="359" frameBorder="0" class="giphy-embed" allowFullScreen></iframe>

### DOM from Milwaukee Upstream.

<iframe src="https://giphy.com/embed/xUOxf1bMsllY6KZ9xC" width="480" height="359" frameBorder="0" class="giphy-embed" allowFullScreen></iframe>

### DOM from eutrophic lake at Veterans Park.

<iframe src="https://giphy.com/embed/xUOxf46Rlm2uLpWVEc" width="480" height="359" frameBorder="0" class="giphy-embed" allowFullScreen></iframe>

# References

Eaton, D. F. (1988) Reference materials for fluorescence measurement. Pure Appl. Chem. 60, 1107-1114.
