---
layout: post
date: 2017-07-19 15:57
categories: Research
title: 2017 Great Lakes Investigation Data Analysis and Presentation
tags: Research
---

<style>
table{
    border-collapse: collapse;
    border-spacing: 0;
    border:2px solid #000000;
}

th{
    border:2px solid #000000;
}

td{
    border:1px solid #000001;
}
</style>

Latest update: 2017-9-20

**R/V**: Blue Heron.

**Sample date**: June 14 ~ 21, 2017.

**Data measurements**: UV-Visable spectrom, EEMs, DOC, DN, FlFFF.

**Sampling sites**:

 <link rel="stylesheet" href="https://unpkg.com/leaflet@1.7.1/dist/leaflet.css"
   integrity="sha512-xodZBNTC5n17Xt2atTPuE1HxjVMSvLVW9ocqUKLsCC5CXdbqCmblAshOMAS6/keqq/sMZMZ19scR4PsZChSR7A=="
   crossorigin=""/>
   
   <script src="https://unpkg.com/leaflet@1.7.1/dist/leaflet.js"
   integrity="sha512-XQoYMqMTK8LvdxXYG3nZ448hOEQiglfqkJs1NOQV44cWnUrBc8PkAOcXy20w0vlaXaVUearIOBhiXZ5V3ynxwA=="
   crossorigin=""></script>

<style>
#mapid { height: 500px; }
</style>

<div id="mapid">
<script>
var mymap = L.map('mapid').setView([44.576071, -88.674484],6);

L.tileLayer('https://api.mapbox.com/styles/v1/{id}/tiles/{z}/{x}/{y}?access_token={accessToken}', {
    attribution: 'Map data &copy; <a href="https://www.openstreetmap.org/">OpenStreetMap</a> contributors, <a href="https://creativecommons.org/licenses/by-sa/2.0/">CC-BY-SA</a>, Imagery © <a href="https://www.mapbox.com/">Mapbox</a>',
    maxZoom: 18,
    id: 'mapbox/streets-v11',
    tileSize: 512,
    zoomOffset: -1,
    accessToken: 'pk.eyJ1IjoiYTU0MTQ0IiwiYSI6ImNrZ2I5NmExczBleTAycnRoMTBveGFvazAifQ.M2spDVYVzk3GOr1yY-5Zdw'
}).addTo(mymap);

var marker1 = L.marker([43.3831,-87.15]).addTo(mymap);
var marker2 =L.marker([45.1261,	-85.8201]).addTo(mymap)
var marker3 =L.marker([42.32,	-86.57]).addTo(mymap)
var marker4 =L.marker([42.4597,	-86.9752]).addTo(mymap)
var marker5 =L.marker([47.4349,	-87.5697]).addTo(mymap)
var marker6 =L.marker([47.0394,	-86.0862]).addTo(mymap)
var marker7 =L.marker([47.1499,	-91.3002]).addTo(mymap)
var marker8 =L.marker([47.1499,	-91.3002]).addTo(mymap)

</script>
</div>


<!-- ![](\image\GL2017\Sampling_map2.jpg) -->


Lake water samples were collected on board the R/V _Blue Heron_ between June 14<sup>th</sup> and 21<sup>st</sup>. Surface water samples were collected using the pump. Deep water samples (S30-278m, S13-125m) were collceted via Niskin bottles amounted on a CTD rossete.

![](\image\GL2017\Table-1.jpg)

## DOC concentration, a<sub>254</sub>, and SUVA<sub>254</sub>

![](\image\GL2017\Graph1.jpg)


![](\image\GL2017\Graph245.jpg)

We found robust linear relationship between CDOM a<sub>254</sub> and DOC in Lake Michigan, but not in Lake Superior due to the consistency of Lake Superior. However, in the colloidal fractionation and < 1kDa fractionation the relationships were not observed in Lake Michigan. But the a<sub>254</sub>-DOC relationship were significant in Lake Superior. DOC concentration and CDOM a<sub>254</sub> values, which are comparatively lower in Lake Superior than Lake Michigan agree with measures in *Zhou et al. (2013)*.   

![](\image\GL2017\DOC-a254-SUVA-surface_bg_clear.jpg)

![](\image\GL2017\Zhengzhen.jpg)

![](\image\GL2017\Table-2.jpg)

## EEMs analysis

![](\image\GL2017\LakeEEMscombination.jpg)

![](\image\GL2017\bix_fix_hix_surface_bg_clear.jpg)

Four FDOM components decomposed by parallel factor analysis are shown below.

 __Component1__ is a typical Humic-like component. It contains __peaks A__ (Ex:260 nm, Em:380~460 nm) and __peaks C__ (Ex:330 nm, Em:420~480 nm).  It was the most intense peak in all fluorescence EEMs.

 __Component 2__ is corresponding to __peaks B__ (Ex:275 nm, Em:310 nm) and/or __peaks T__ (Ex:275 nm, Em:350 nm). It seems like a combination of __peaks T__ and __peaks B__. Whatever it would be a Protein-like fluorophore.

The second highest peak from __Component 3__ is corresponding to __peaks M__ (Ex: 312 nm, Em:380~420 nm).  It is probably a **humic-like** component.

__Component 4__ is probably a noise-derived component.

![](\image\GL2017\Fluorescence-EEM-Plot-of-components_2.jpg)

### Distribution of C1~C4

High correlation relationship is observed between **Component 1** and **Component 3**, which indicates similar source of these two components. Distribution of **Component 2** demonstrated more **autochthonous** fluorescence matter in Lake Michigan than Lake Superior.

![](\image\GL2017\C1-C3_bg_clear.jpg)

### Correlation between parameters

![](\image\GL2017\Correlation.jpg)

## Size distribution of colloids in the Great Lakes

**Concentration Normalization completed.**

Hydrodynamic diameters of the dissolved organic colloids (UV<sub>254</sub>)

![](\image\GL2017\Multiple-samples---Hydrodynamic-diameter-nm-UV1-lake2017.jpg)

Hydrodynamic diameters of the __Protein-like__ colloids

The small peak disappeared in Sample **S23-0m** and **Sample S22B-0m**.

![](\image\GL2017\Multiple-samples---Hydrodynamic-diameter-nm-FLD2-lake2017.jpg)

Hydrodynamic diameters of the __Humic-like__ colloids

![](\image\GL2017\Multiple-samples---Hydrodynamic-diameter-(nm)-FLD1-lake2017.jpg)

## Molecular weights of peak in size chromotography

$$ M_n = \frac{\sum M_i \cdot n_i}{\sum n_i}$$

$$ M_w = \frac{\sum M_i \cdot w_i}{\sum w_i} = \frac{\sum M_i^2 \cdot n_i}{\sum M_i \cdot n_i}$$

$$ DPI = \frac{M_w}{M_n}$$

![](\image\GL2017\Table-3.jpg)

<!-- ![](\image\GL2017\Mwcalculation.jpg) -->

Integration - UV1

![](\image\GL2017\Multiple-samples---Integrations-of-each-size-intervals-Da-UV1.jpg)

Integration FLD1 __Huimic-like__

1 One peak;

2 Normalized distribution;

![](\image\GL2017\Multiple-samples---Integrations-of-each-size-intervals-Da-FLD1.jpg)

Integration -FLD2 __Protein-like__

![](\image\GL2017\Multiple-samples---Integrations-of-each-size-intervals-Da-FLD2.jpg)

## Pie charts

UV1
![](\image\GL2017\Multiple-samples---Pie-Chartss-of-each-size-intervals-Da-UV1.jpg)

__Huimic-like__ (FLD1)
![](\image\GL2017\Multiple-samples---Pie-Chartss-of-each-size-intervals-Da-FLD1.jpg)

__Protein-like__ (FLD2)
![](\image\GL2017\Multiple-samples---Pie-Chartss-of-each-size-intervals-Da-FLD2.jpg)

HMW fractionation (>100 kDa) in protein-like FDOM occupied averagely more than half of the integration (57.32%) in Lake Michigan. Meanwhile, the largest protein-like fractionation (>100 kDa) has greatest proportion of FDOM integration chromotography.

|       Lake Michigan       |       |      Lake Superior      |
|:-------------------------:|-------:|:-------------:|---------:|
| UV1                       |       |               |         |
| 1-5kDa                                                      |
| S3-0m                     | 44.04 | S23-0m        | 46.64   |
| KS103-0m                  | 44.02 | S22B-0m       | 51.09   |
| S13.5-0m                  | 38.21 | S30-0m        | 48.25   |
| S13-125m                  | 38.13 | S30-278m      | 48.79   |
| Average                   | 41.1  | Average       | 48.69 |
| > 100 kDa                 |       |               |         |
| S3-0m                     | 19.42 | S23-0m        | 12.21   |
| KS103-0m                  | 19.15 | S22B-0m       | 7       |
| S13.5-0m                  | 30.03 | S30-0m        | 6.75    |
| S13-125m                  | 26.81 | S30-278m      | 5       |
| Average                   | 23.85 | Average       | 7.74    |
| Humic-like fluorescence   |       |               |         |
| 1-5kDa                    |       |               |         |
| S3-0m                     | 51.6  | S23-0m        | 55.24   |
| KS103-0m                  | 52.93 | S22B-0m       | 58.71   |
| S13.5-0m                  | 50.66 | S30-0m        | 55.11   |
| S13-125m                  | 52.06 | S30-278m      | 55.66   |
| Average                   | 51.81 | Average       | 56.18   |
| > 100 kDa                 |       |               |         |
| S3-0m                     | 5.36  | S23-0m        | 4.45    |
| KS103-0m                  | 6     | S22B-0m       | 4.24    |
| S13.5-0m                  | 7.31  | S30-0m        | 3.93    |
| S13-125m                  | 6.45  | S30-278m      | 2.19    |
| Average                   | 6.28  | Average       | 3.70    |
| Protein-like fluorescence |       |               |         |
| 1-5kDa                    |       |               |         |
| S3-0m                     | 28.06 | S23-0m        | 27.46   |
| KS103-0m                  | 13.07 | S22B-0m       | 36.24   |
| S13.5-0m                  | 24.5  | S30-0m        | 34.14   |
| S13-125m                  | 27.36 | S30-278m      | 27.31   |
| Average                   | 23.25 | Average       | 31.29   |
| > 100 kDa                 |       |               |         |
| S3-0m                     | 50.49 | S23-0m        | 45.7    |
| KS103-0m                  | 72.21 | S22B-0m       | 30.16   |
| S13.5-0m                  | 59.49 | S30-0m        | 30.65   |
| S13-125m                  | 47.07 | S30-278m      | 45      |
| Average                   | 57.32 | Average       | 37.88   |

## Pie charts

UV1
![](\image\GL2017\Multiple-samples---Pie-Chartss-of-each-size-intervals-Da-_Combined_with_LMWUV1.jpg)

__Huimic-like__ (FLD1)
![](\image\GL2017\Multiple-samples---Pie-Chartss-of-each-size-intervals-Da-_Combined_with_LMWFLD1.jpg)

__Protein-like__ (FLD2)
![](\image\GL2017\Multiple-samples---Pie-Chartss-of-each-size-intervals-Da-_Combined_with_LMWFLD2.jpg)

## PCA Analysis

![](\image\GL2017\PCA-Analysis_esclipes.jpg)

## Summary
![](\image\GL2017\Table-4.jpg)
