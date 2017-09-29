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
}).addTo(mymap);

var marker1 = L.marker([43.025392,-87.903591]).addTo(mymap);
marker1.bindPopup("<b>Downstream</br></b>Estuary").openPopup();

var marker2 =L.marker([43.133424, -87.928420]).addTo(mymap)
marker2.bindPopup("<b>Upstream</b><br>Kletzsch Park.").openPopup();

</script>
</div>
