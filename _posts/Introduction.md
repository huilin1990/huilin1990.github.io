---
layout: post
date: 2020-7-12 12:08
categories: Research
title: Veterans Lagoon
tags: Research
---
## Working title: temperature and microbial driven inland freshwater ecosystem.

<b> Key words:</b> algal bloom; bacteria; cyanobacteria; dissolved organic matter; ultrafiltration; size distribution

hypothesis: cyanobacteria 
when cyanobacteria be heterotrophic and when are they autotropic?

# Introduction

# Method

## Study site and sample collection

 <link rel="stylesheet" href="https://unpkg.com/leaflet@1.7.1/dist/leaflet.css"
   integrity="sha512-xodZBNTC5n17Xt2atTPuE1HxjVMSvLVW9ocqUKLsCC5CXdbqCmblAshOMAS6/keqq/sMZMZ19scR4PsZChSR7A=="
   crossorigin=""/>
   
   <script src="https://unpkg.com/leaflet@1.7.1/dist/leaflet.js"
   integrity="sha512-XQoYMqMTK8LvdxXYG3nZ448hOEQiglfqkJs1NOQV44cWnUrBc8PkAOcXy20w0vlaXaVUearIOBhiXZ5V3ynxwA=="
   crossorigin=""></script>

<style>
#mapid { height: 300px; }
</style>

<div id="mapid">
<script>
var mymap = L.map('mapid').setView([43.047043, -87.894789],15);

L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 20,
}).addTo(mymap);

var marker1 = L.marker([43.049837,-87.890379]).addTo(mymap);
var marker2 =L.marker([43.044197,-87.894670]).addTo(mymap)

</script>
</div>


Veterans Lagoon (VL) is a small (14.7 acres), shallow (averagely 1.5 m), well-mixed enclosed lagoon within the Veterans County Park, close to the downtown metropolitan Milwaukee, WI. The absence of surface runoff and point-source anthropogenic inputs make this lagoon a relatively simple system, where 68.2% of water input is from surface precipitation. The nearly one-year hydraulic time (0.9 yr) makes it an ideal natural mesocosm for documenting the cycling of DOM during phytoplankton blooms. 

We selected two sampling points (north and south) in the lagoon. Surface water samples were collected weekly or biweekly between March 11th, 2019 and Jan 10th, 2020, using a lab-made water sampler and pre-rinsed HDPE bottles. Water samples were immediately filtered using pre-combusted 0.7 μm GF/F filters (Whatman) after shipping back to lab. The GF/F filters were stored frozen before further measurements. 

## Sample analysis 

An aliquot of the filtrate (180 ml) was size-fractionated into < 1 kDa, 1-10 kDa, and 10 kDa -0.7μm three fractions using a stirred cell ultrafiltration system (Amicon 8200) with 1 and 10 kDa membrane (regenerated cellulose, Millipore YM1, 63.5-mm diameter). Details of the procedures are described in Xu & Guo, (2017). 

Dissolved Organic Carbon (DOC) samples were analyzed by high-temperature catalytic oxidation using a Shimadzu TOC-L Total Organic Carbon Analyzer (Guo et al., 1994). Particulate Organic Carbon (POC) samples and Particulate Nitrogen (PN) samples were dried at 60 ℃ before analysis on ECS 4010 elemental analyzer (Costech instruments). Stable isotopes δ13C and δ15N were measured using Delta V Plus isotope ratio mass spectrometry. Chlorophyll a (Chl a) concentration was analyzed by standard spectrophotometric method. (Strickland & Parsons, 1972). 

# Results

## Weather condition in the sampling area
  
Figure 1. Left Panel: Time series of daily air temperature (gray dots), weekly averaged air temperature (blue dots), in situ measured water temperature (red dots) and predicted water temperature (orange dots). Right panel: Historical records of precipitation, including rainfall (blue bars) and snowfall (red bars), were presented.

Some of the water temperature was missing due to the dysfunctionality of in situ measurement equipment. According to the historical weather data, the daily average temperature and weekly average temperature are close to the in situ measured water temperature (Figure 1). Here we predict the unknown water temperature using daily or weekly average air temperature with a least square regression algorithm. The R-squares of the two linear regression models demonstrated that average daily air temperature can better predict water temperature than weekly average air temperature can (Figure S1). Therefore, historical daily average air temperature was used to predict the in situ water temperature.

## Seasonal variations of DOM concentration

CDOM a254 and DOC concentration were keeping increasing in the spring (March - May, 2019, Figure 3a&b). They remain stable in the summer and fall (June-November 2019) except the spikes observed in the deep November. After the spikes CDOM a254 and DOC concentration decreased dramatically to the winter baseline. Except the spike in the November, the seasonality of DOC was highly similar as the temperature variation; two little bumps in 17th July and 6th September were corresponding to the hottest days in the downtown Milwaukee. The TDN concentration was generally invariant except the spike in the November which was 54.6 ± 5.4 μmol-N/L. 

## Seasonal variation of DOM properties

CDOM spectral slope (s275-295) was low in summer, but high in winter, which indicated that DOM molecular weight was relatively low in the winter and high in the summer (Figure 4a). SUVA254 exhibits a relatively stable time-series change (Figure 4b), except the outliers in the November. This indicated that the outbreak of DOM in the November was of high molecular size, but low aromaticity. Unlike other terrestrial input dominated water environments, this freshwater ecosystem contained autochthonous and allochthonous DOM, which was indicated by the scattering patterns shown in the DOC vs. CDOM a254 relationship (Figure 4c). As the Figure 4c shown, the scatter points in the summer are more converged than those from the cold seasons, which was due to the terrigenous DOM input in the summertime. 

In the summer, the BIX was high while the HIX was relatively low (Figure 5). There was no spike observed in the time-series variation of BIX. However, HIX is relatively insistent except the valley in the November. 

## Size fractionated DOM

DOM is a heterogeneous complex with various chemicals and fluorophores. A few EEM contours of several representative samples are presented here (Figure S3). Fluorescence properties of DOM were highly size-dependent. The humic-like fluorophores were majorly presented in < 1 kDa, 1-10 kDa size fractions (Figure 7). The protein-like fluorophore was obviously in 10 kDa–0.7 μm fraction. this observation was highly consistent with other studies conducted before (Lin and Guo 2019).

The < 1 kDa fraction and 1-10 kDa fraction were single peak distribution (< 1 kDa maximum in July; 1-10 kDa maximum in September), while the > 10 kDa fraction was bimodal distribution with two maxima in May and November. 1-10 kDa was the largest fraction among these three. 

Fluorescence intensities of all components in < 1 kDa fraction were increasing from March to July 2019, then decreased from July 2019 to January 2020. As for 1-10 kDa size fraction, the C1 and C2 were more abundant than C3 and C4. The > 10 kDa fraction was quite intriguing. In March, May, July and September, the protein-like C4 contributed much more than other humic-like components. However, in November and January, humic-like components were dominant in the > 10 kDa fraction.   

# Discussion

## Fluorescent components

## one-year ecological succession/temperature/microbial driven ecosystem

## carbon and nitrogen ratio/stable isotopes

## DOM properties in different molecular weight

# Conclusion

