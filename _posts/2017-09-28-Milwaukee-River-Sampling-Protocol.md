---
layout: post
date: 2017-9-28 17:12
categories: Research
title: Milwaukee River Sampling Protocol
---
<style>
#mapid { height: 600px; }
</style>

<div id="mapid">
<script>
var mymap = L.map('mapid').setView([43.07, -87.92],12);

var Hydda_Base = L.tileLayer('https://{s}.tile.openstreetmap.se/hydda/base/{z}/{x}/{y}.png', {
	maxZoom: 18,
	attribution: 'Tiles courtesy of <a href="http://openstreetmap.se/" target="_blank">OpenStreetMap Sweden</a> &mdash; Map data &copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
}).addTo(mymap);_

var marker1 = L.marker([43.025392,-87.903591]).addTo(mymap);
marker1.bindPopup("<b>Estuary</br></b>Milwaukee County Boat Launch").openPopup();

var marker2 =L.marker([43.133424, -87.928420]).addTo(mymap)
marker2.bindPopup("<b>Upstream</b><br>Kletzsch Park.").openPopup();

var marker3 =L.marker([43.0489, -87.8906]).addTo(mymap)
marker2.bindPopup("<b>Euphotic Lake</b><br>Veterans Park.").openPopup();

var marker4 =L.marker([43.03529, -87.9101532]).addTo(mymap)
marker2.bindPopup("<b>Downstream</b><br>Milwaukee Public Market.").openPopup();

</script>

## Methods

### Calibrate four online fluorescence detectors and two UV detectors.

Excitation and emission wavelength were set to 310/425.

</div>

<iframe width="900" height="800" frameborder="0" scrolling="no" src="//plot.ly/~a54144/4.embed"></iframe>

<iframe width="900" height="800" frameborder="0" scrolling="no" src="//plot.ly/~a54144/8.embed"></iframe>

<iframe width="900" height="800" frameborder="0" scrolling="no" src="//plot.ly/~a54144/10.embed"></iframe>
