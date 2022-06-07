---
layout: post
date: 2018-7-12 12:08
categories: Research
title: Fox River-Green Bay estuary investigation
tags: Research
---
# Study the size and composition of dissolved organic matter in a negative estuary using one sample FlFFF-EEM-PARAFAC technique

# Abstract

Molecular size plays an important role in dissolved organic matter (DOM) biogeochemistry. It has been widely investigated in marine coastal estuaries. However, it is still unclear about the DOM size in a negative estuary and its relationship with the fluorescent dissolved organic matter (FDOM) where inorganic ion density declines from river to open water. Here we use flow field flow fractionation (FlFFF) coupling to fluorescence emission excitation (EEM) spectroscopy and further parallel factor analysis (PARAFAC) to determine the size and fluorescent composition of DOM in the Fox River – Green Bay estuary. Water samples from a six-station transect were collected and measured using the method. Size spectra of UV254 and allochthonous FDOM Fluo350/450 were highly similar, while the autochthonous DOM Fluo275/340 has a great variety. One sample FlFFF-EEM-PARAFAC generate four fluorescent components except the Green Bay open water, where only three components were generated. Inter-sample comparison and identification ensure that totally four components were in this ecosystem. Two ubiquitous humic-like components were conservative mixing in the estuary while two protein-like components increased with the declining specific conductivity. Size of DOM remained constant in the estuary, while the composition of DOM changed due to the change of source and sink.

# Introduction

Dissolved organic matter (DOM) in aquatic environments plays an important role in the global carbon cycle because of its huge amount and dynamic reactivity (Hansell and Carlson 2002). It has been recognized that DOM strongly participates in a series of critical environmental and ecological processes particularly in the biogeochemical cycling (Coble 2007; Coble et al. 2014). Previous studies showed that several biogeochemical processes were significantly affected by DOM properties. For example, the size of DOM influences the coagulation, flocculation, and precipitation of colloidal DOM and its complexation abilities with trace metals (Guo et al. 2000; Santschi 2018). Meanwhile, DOM composition is one of the most important DOM properties reflecting the reactivity and age of DOM (Benner et al. 1997). 
The size and composition of DOM have been widely investigated in marine estuaries (Guo and Santschi 2007; Baalousha et al. 2011). However, a limited number of studies have reported the DOM size and composition in the lacustrine estuaries, especially negative estuaries. Negative estuaries are the estuaries where inorganic ion strength decreases from river to open water (Xu et al. 2018a). Different with the increasing salinity gradient in normal marine estuaries, negative estuaries have significantly different chemical environments. Generally, the size of DOM decreases from river to open water with increasing age and decreasing reactivity (Benner and Amon 2015). In marine estuaries, flocculation makes aggregated colloids removed, leading to the decline of the DOM size. Meanwhile, based on the double layer model of colloids (DLVO theory), increase of ion density of ambient solution would compress the size of colloids in it, and vice versa. Thus, it was expected that the diluted inorganic ion strength would increase the thickness of the double electric layer of DOM. Therefore, unlike the DOM in marine estuaries, the size of DOM is expected to increase in a negative estuary.
Currently, optical determinations (e.g UV-visible absorbance spectroscopy, infrared spectroscopy, and fluorescence spectroscopy) have been successfully used to study the concentration and nature of DOM in many environmental ecosystems and trace DOM sources. Particularly, fluorescence spectroscopy has been widely used since it provides information about both DOM abundance and fluorescent components in DOM. Coupling with parallel factor analysis (PARAFAC), a statistical tool to deconvolute excitation emission matrices (EEM) spectra into several components, EEM deliver fingerprints information about DOM with various sources (Stedmon et al. 2003). It provides a powerful tool to characterize DOM components both quantitatively and qualitatively. However, due the fact that PARAFAC requires a large amount of sample set, sometimes PARAFAC is not suitable for small area investigation. To address this issue, one sample FlFFF-EEM-PARAFAC was developed to characterize the size distribution and fluorescent DOM components within one individual sample (Lin and Guo 2020).  
In this study, the Fox River plume estuary was selected as our study area which is one of the biggest negative estuaries in the world. We investigated a transect of the negative estuary including six stations from the Fox River downstream to the southern Green Bay open water. Surface water samples were collected, filtered, ultrafiltration concentrated. Size and composition of DOM were determined using the one sample FlFFF-EEM-PARAFAC method. Our objectives were to (1) apply the one sample FlFFF-EEM-PARAFAC technique in one natural ecosystem and compare this method with the traditional PARAFAC; (2) evaluate DOM size and composition change in a negative estuary, and further exploring the potential factors causing these variations.


 
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
var mymap = L.map('mapid').setView([44.57, -88],11);

L.tileLayer('https://api.mapbox.com/styles/v1/{id}/tiles/{z}/{x}/{y}?access_token={accessToken}', {
    attribution: 'Map data &copy; <a href="https://www.openstreetmap.org/">OpenStreetMap</a> contributors, <a href="https://creativecommons.org/licenses/by-sa/2.0/">CC-BY-SA</a>, Imagery © <a href="https://www.mapbox.com/">Mapbox</a>',
    maxZoom: 18,
    id: 'mapbox/streets-v11',
    tileSize: 512,
    zoomOffset: -1,
    accessToken: 'pk.eyJ1IjoiYTU0MTQ0IiwiYSI6ImNrZ2I5NmExczBleTAycnRoMTBveGFvazAifQ.M2spDVYVzk3GOr1yY-5Zdw'
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

## Ultrafiltration

To pre-concentration and isolate > 1 kDa DOM (commonly regarded as colloidal DOM) for FlFFF, stirred cell ultrafiltration was conducted within three days. A stirred cell unit (Amicon 8200) with 1 kDa membrane (regenerated cellulose, YM1, Millipore) was used. Detailed method has been described previously (Helms et al. 2008; Lin and Guo 2016). Briefly, the membrane was rinsed with 0.05 M NaOH, and deionized (DI) water before each water sample loading. About 20 ml water sample was loaded and 10 ml of them was penetrated through the membrane to pre-conditionate the membrane. An originally 180 ml filtrate was ultra-filtered to 18 ml concentrated retentate (concentration factor = 10). The volume of retentate was monitored to keep it from over-filtering. During the ultrafiltration, high pressure (60 psi) zero grade nitrogen gas (Airgas), providing air pressure, was applied in the stirred cell unit to make low molecular weight DOM penetrate through the ultrafiltration membrane. The final 18 ml retentates were stored in 4°C fridge until FlFFF analysis within 4 days.  

## DOC and DOM optical properties measurements

DOC concentrations were measured by Shimadzu TOC-L analyzer. Details of DOC measurements were described in previous studies (Zhou et al. 2013). To remove inorganic carbon in water, samples were acidified to pH 2 before measurements. Calibration curves were made before sample measurements. DI water samples were measured every five samples to monitor the background signals. Internal standards were measured every ten samples for quality assurance. 
UV-visible spectrophotometer (Agilent 8453) provides absorbance spectra from ultraviolet (i.e. 200 nm) to visible light (i.e. 900 nm) with a 10-mm quartz cuvette. Ultrapure water was used as reference blank, and the refractive index effect was corrected (Weishaar et al. 2003; DeVilbiss et al. 2016). Absorption coefficient at 254 nm (a<sub>254</sub>, in m<sup>-1</sup>), commonly recognized as DOM concentration indicator due to its linear correlation with DOC concentration in terrigenous DOM dominant areas (Fichot and Benner, 2011), was calculated using the following equation: 

a<sub>254</sub> = 2.303 × A<sub>254</sub>/l

where A<sub>254</sub> is absorbance at 254 nm, and l is the light path length of the cuvette (in meter). Spectral slope (s<sub>275-295</sub>) was calculated using a non-linear regression to fit the absorption spectra ranging from 275 nm to 295 nm (Fichot and Benner, 2012) based on this equation: 

a<sub>λ</sub>=a<sub>280</sub> e<sup>s<sub>275-295</sub>(λ-280)</sup>

, where λ is the wavelength, a<sub>280</sub> is the absorption coefficient at 280 nm, aλ is absorption coefficient at wavelength λ and s275-295 is the spectral slope between 275 nm and 295 nm, which shows inversely correlated with DOM molecular weights (Fichot and Benner, 2012). SUVA254 (in L mg-1 m-1), an indicator of aromaticity, was calculated using the following equation: 

SUVA<sub>254</sub> = A<sub>254</sub>/DOC

where A<sub>254</sub> is the absorbance at 254 nm and DOC (in mg/L) is the concentration of dissolved organic carbon (Weishaar et al. 2003). Absorption ratio between λ = 250 nm and λ = 365 nm (known as E2:E3 ratio) was used to track relative molecular size change, while the ratio of absorption at λ = 465 nm to λ = 665 nm (known as E4:E6) could be used as an CDOM aromaticity indicator (Helms et al. 2008). 
EEM provides fluorescent fingerprint patterns of DOM. EEM measurements were carried out using a Horiba Fluoromax-4 spectrofluorometer (Japan) in 3D scan mode with a 10 mm quartz cuvette. Excitation wavelength (Ex) ranged from 220 nm to 480 nm with 5 nm increment, while emission wavelength (Em) ranged from 260 nm to 600 nm with 2 nm increment. DI water was scanned for each measurement batch as a blank reference. To eliminate the inner filter effect, water samples were diluted using ultrapure water until the A254 is no larger than 0.02. First order and second order of Rayleigh scattering peaks and Raman scattering peaks were removed, and every EEM was double checked with visual inspection (Zhou et al. 2016a). A series of quinine sulfate solutions were determined to calibrate fluorescence intensities, and quinine sulfate equivalent (QSE) was used as a dimension of the fluorescence.
Fluorescence indices derived from EEM data have been used to explore potential DOM source that might be ignored using empirical peak-based method (Huguet et al., 2009; Yang et al., 2012; Zsolnay et al., 1999). Biological index (BIX) and humification index (HIX) are two dimensionless indicators showing autochthonous source and allochthonous source, respectively. BIX was calculated using the following equation:

BIX= (I_(em=380) ⁄ I_(em=430))<sub>ex=310 nm</sub>

, where the I_em is the fluorescence intensity at a specific Em. HIX was calculated from an emission spectrum where excitation wavelength is 254 nm: 

HIX= (I_(em=435-480)⁄I_(em=300-345) )_(ex=254)

, where the I_(em=435-480) is integrated fluorescence intensities from a wavelength band from 435 nm to 480 nm, and I_(em=300-345) is integrated fluorescence intensities from 300 nm to 345 nm (Huguet et al. 2009).

## One sample FlFFF-EEM-PARAFAC

Colloidal DOM in water samples were size fractionated using a FlFFF system (Postnova, Salt Lake City, UT). Procedures for injections and separation were thoroughly described in previous studies (Zhou et al. 2016b; Lin and Guo 2020). Briefly, ultrafiltration-concentrated water samples were injected into the system using a rinsed plastic syringe. The injected sample was carried to the FlFFF separation channel with carrier solution, which is made of 10 mM NaCl, 5 mM H3BO3, and pH = 8 (adjusted using NaOH). The size spectrum was calibrated using several molecular-weight-known protein standards (e.g. Bovine Serum Albumin, ovalbumin, Vitamin B12, etc.). Size distribution spectra were obtained using online optical detectors including a two-channel UV-vis spectroscopy (SPD-20A, Shimadzu, Japan) and two fluorescence detectors (RF-20A, Shimadzu, Japan). The online UV-visible detector measured the absorbance at a fixed λ = 254 nm. Two fluorometers targeted at Ex/Em = 350/450 nm (Fluor350/450) and Ex/Em = 275/340 nm (Fluor275/340), which empirically indicated as the UVC humic-like fluorophore (Peak C) and protein-like fluorophore (Peak T).
One sample FlFFF-EEM-PARAFAC method was thoroughly described in (Lin and Guo 2020). Briefly, fractionated sub-samples were collected manually at the end of FlFFF separation in every minute. Injections were repeated triply to collect adequate subsample fractions for EEM measurements. The subsample fractions were collected into pre-acid-rinsed 5 ml centrifugal tubes and measured offline. The EEM measurement procedures for the subsample fractions are same as the EEM measurements for the bulk samples. PARAFAC was performed to mathematically deconvolute EEM database according to following equation: 
x_ijk= ∑_(f=1)^F▒〖a_if b_jf c_kf 〗+e_ijk
The xijk is the fluorescence signal intensity of sample i measured at Em = j and Ex = k. In the right side of equation is the sum of factorized components and the model residuals (eijk). aif is model scores, proportionated to the fluorescence intensity, of the component f in the sample i. bjf, is model-estimated excitation loadings of component f at λEm = j, while ckf¬ is model-estimated emission loadings of the component f at λEx = k. Non-negativity rules were applied to established models in order to guarantee all positive values in scores (aif) and spectra loadings (bjf and ckf). As PARAFAC is an unsupervised algorithm, a half-split validation is a reliable approach to evaluate the model results (Stedmon and Bro 2008). Number of components was evaluated and eventually determined by sum of squared errors. Ten random initialized model were developed and compared using a convergence criterion setting to 10-7 to optimize the model. 
Tucker’s congruence coefficient (TCC) was used in the half-split validation. In this study, it was also used to statistically compare and identify components. It is an index to evaluate the similarity between factors calculated from the following equation: 
TCC=  (∑▒XY)/√(∑▒X^2  ∑▒Y^2 )
, where X and Y represents the excitation loadings and emission loadings from two models. Generally, a congruence coefficient of 0.90 is interpreted as a high degree of factor similarity, while a coefficient of 0.95 or higher indicates that the factors are virtually identical (Kathleen R. Murphy et al., 2014; Stedmon and Bro, 2008). To ensure our model reliable, the threshold of TCC in the half-split validation was set at 0.95, but it was set at 0.90 in the inter-model comparison. The drEEM toolbox (version 0.5.0) was used to perform the PARAFAC analysis on the Matlab (R2018b) platform (Murphy et al., 2013).

# Results
## Bulk DOM characteristics
In the Fox River - Green Bay estuarine area, DOC concentration ranged from 441.1 μmol/L to 868.8 μmol/L, and a254 ranged from 27.7 m-1 to 64.2 m-1, which were consistent with observations reported previously (Klump et al. 2009; Lin et al. 2016b; Xu et al. 2018a). Along with the declining specific conductivity gradient, DOC and CDOM a254 were diluted conservatively (Figure 2) except the first sampling point, which, as mentioned above, was from a tributary East River draining into the Fox River downstream. The aromaticity indicators (SUVA254 and E4:E6) and humification indicators (HIX) also decreased from the river to the bay, while E2:E3 and s275-295, the molecular weight indicators, showed opposite patterns (Figure 2). These quantitative and qualitative optical properties demonstrated that not only the DOM concentration diluted conservatively, but also the DOM compositional structure changed along the dilution. Although the onshore Chlorophyll a concentration was exceedingly higher than those in the open Green Bay (Figure 1), the BIX showed an asynchronous pattern, which gradually increased with the decreasing specific conductivity gradient. These optical parameters were consistent with those observations from previous studies (Xu et al. 2018a). 

## DOM molecular size distribution in the estuary
Colloidal DOC (>1 kDa) was 66.0% to 76.7% of bulk DOC with an average of 71.3±4.1%, while colloidal CDOM a254 was 65.2% to 78.0% of bulk CDOM a254 with an average of 72.7±5.0% (Figure S1). Both colloidal DOC and CDOM a254 stayed steady along this estuary. However, the percentage of colloidal DOC is significantly larger than those reported by Xu et al. (2018a). The major reason for the large difference is the gap between authentic membranes cutoffs and the cutoffs estimated by manufactures. As calibrated by Xu and Guo (2017), the authentic membrane cutoff of a manufacture-rated 1 kDa membrane in a centrifugal ultrafiltration unit is 2.5 kDa. It would significantly underestimate the colloidal fraction (> 1 kDa) of DOM in natural fresh waters since the humic-like DOM is mostly within the 1-3 kDa size fraction (Lin and Guo 2020). Moreover, different sampling season might be another reason for the difference. The waters from this investigation contained more autochthonous DOM from algae and phytoplankton due to summer blooms while in the May 2016 more soil-leached humic substances contributed to < 1kDa and 1-3 kDa DOM fractions.
 
Size spectra from FlFFF system showed that UV254 (bulk DOM, Figure S2) and Fluor350/450 (humic-like, Figure S3) exhibited a single-narrow-peak fractogram, while Fluor275/340 (protein-like, Figure S4) was a single peak with a shoulder tailing toward a larger molecular size. Normalized size fractogram of UV254, Fluor350/450 and Fluor275/340 were highly similar between samples (TCC >0.99 for UV254 and Fluor350/450, TCC>0.90 for Fluor275/340, Table S1), although the major peak intensities were coherent with the declining DOC concentration and CDOM a254 from the river to open bay. The integrations of the fine-divided size intervals showed that Fluor275/340 (protein-like) was dominated in 100 kDa -0.7μm fraction (Figure S4), while UV254 (bulk DOM) and Fluor350/450 (humic-like) were majorly in the relatively small size ranges i.e. 1-3 kDa and 3-10 kDa (Figure S2 and Figure S3).
 
To compare with previous studies, the fine-divided size fractions were integrated into four major size fractions: 0.3-1 kDa, 1-3 kDa, 3-10 kDa, and >10 kDa. Obviously, conservative mixing behaviors were shown in terms of UV254 and Fluor350/450; all integrated UV254 and Fluor350/450 size fractions were linearly correlated with the specific conductivity (n=6, r > 0.882, p<0.02, Figure 3 (a) and (b)). The UV254 in Station 6 was 54% of the UV254 in Station 1, while the humic-like fluorescence (Fluor350/450) in Station 6 was 37% of Fluor350/450 in Station 1. As for the Fluor275/340, the largest fraction (>10 kDa) was the most abundant fraction among these size fractions (> 60%, Figure 3 (c)). No significant conservative dilution was clearly observed along the estuary. How much autochthonous protein-like DOM was added along the estuary? To answer this question, we assumed that the part of protein-like DOM from terrestrial input diluted linearly along the estuary like UV254. To eliminate the impacts from this part of DOM, the linear diluted terrestrial Fluor275/340 was removed from the bulk Fluor275/340. The remaining Fluor275/340 could be regarded as the net autochthonous addition provided by algal and microbial activities. From Station 2 to Station 6, the percentage of the autochthonous Fluor275/340 addition are 19.4%, 11.2%, 35.3%, 37.0%, and 30.0% of the bulk Fluor275/340, which indicated that the autochthonous protein-like DOM contribution in offshore areas (> 30%, Station 4, 5 and 6) is larger than those in onshore areas (< 20%, Station 1,2 and 3).
In light of the relative fluorescent intensity of each size fraction, all three DOM indicators remained stable in the estuary (Figure 3 (d), (e) and (f)). For all size fraction of UV254 and Fluor350/450, coefficient of variations (CV) were below 10%, while for the Fluor275/340, CV were under 20%. It implied that for all size fractions, the size distribution remained constant through the estuary, which implied that the colloidal DOM size suffered no substantial alteration within this negative estuary.

## EEM and PARAFAC-derived fluorescent components

The conservative mixing behavior was observed from the fluorescence maximum (Fmax) of EEMs as well (n=6, r=0.965, p<0.05, Figure S5). Although the fluorescent DOM concentration was diluted conservatively, the EEM contour patterns were highly similar between each other. Obviously, Peak A (Ex/Em = 260/400-460 nm) and Peak C (Ex/Em = 320-360/400-460 nm) are dominant on these EEM patterns, which are ubiquitous humic-like fluorophores among the freshwater ecosystems (Coble, 2007; Xu, Lin, et al., 2018; Xu and Guo, 2017; Zhou et al., 2013; Zhou, Guo, et al., 2016; Zhou, Stolpe, et al., 2016). Based on the increasing BIX along the estuary (Figure 2), autochthonous fluorophores were expected to emerge on EEM at the open water end, but none was observed, because the fluorescence from autochthonous DOM (e.g. Peak T and Peak B) is somewhat overwhelmed by the prevailing terrestrial fluorophores. Thus, the one sample FlFFF-EEM-PARAFAC method is in need to decompose the EEM spectra and unravel the underlying components. 
Using the one sample FlFFF-EEM-PARAFAC technique, four-component models were validated for every water sample except the Station 6 sample, in which only a three-component model was validated (Figure 4). To compare and identify these fluorescent components, inter-model comparisons and fluorescence components identifications were performed using the TCC method (Table S2). These components were named after their characteristic emission peak from their emission loadings, e.g. C475 for the first component in Station 1 (Stedmon and Bro, 2008). C475, C320, C410 and C290 were then identified from those components (Figure 5). C475 and C410 are humic-like fluorescent components which were ubiquitous in natural freshwaters (Coble et al. 1998; Stedmon and Markager 2005; Murphy et al. 2018b; Wünsch et al. 2019). According to the conventional peak pick-up method, C475 was a combination of Peak A and Peak C which are UVC and UVA humic-like fluorophores. Its Em loadings from all six samples were highly similar, while its Ex loading maximum varied from 435 nm to 475 nm (Figure 5 (b)). The most deviated Ex loading spectra was of Station 6 model, which contained only three components. C410 was a combination of Peak M and Peak A. It has been reported that C410 was derived from microbial activities, and it correlates to DOM exported from agricultural catchments, possibly resulting from widely-used organic fertilizer on fields (Stedmon and Markager, 2005). Additionally, it is worth noted that C410 could not be factorized in Station 6. These two humic-like components were highly similar with F450 and F420, which were recently reported as ubiquitous components in aquatic environments (Murphy et al. 2018b). The other two fluorescent components are both UVB protein-like autochthonous components. C320 has similar fluorescence characteristics to the tryptophan-like fluorophore (Peak T) detected in several aquatic ecosystems, and C290 resembles the tyrosine-like peak (Peak B) in the Em < 300 nm area (Coble, 1996; Stedmon et al., 2003; Stedmon and Markager, 2005).
 
To better interpret the mixing behavior of each component in the negative estuary, fluorescence intensities of subsamples in each station were summarized. Fmax, converted from PARAFAC model scores, represents the maximum intensity of each component. Fmax of each component were integrated from subsamples in each station (Figure 6 (a)). The humic-like components (C475 and C410) were overwhelming in all 6 stations, while the protein-like components (C320 and C290) fluoresced relatively less. Significant negative linear correlations were found between summarized Fmax (∑Fmax) and specific conductivity in C475, C410 and C320 (n=6, p<0.05, Table S3), though C320 is a protein-like component. The behaviors of the two humic-like components (C475, C410) were consistent with the decreasing HIX (Figure 2), despite that the C410 was absent in the Station 6. The C290 increased minorly along the decreasing conductivity gradient although no significant linear correlation was found between them (Figure 6, Table S3).
Figure 6 (b) shows the relative intensity of these fluorescent components from Station 1 to Station 6. The component percentage was calculated using the following equation:
Component percentage (%) =  (∑▒F_max )/(∑_(i=1)^4▒〖(〖∑▒F_max )〗_i 〗)
C475, varying between 44.8% and 55.2%, stayed relatively constant in the estuary. C410 gradually decreased from 36.0 % to 21.9 % except the station 6. Humic-like fluorescent components (C475 and C410) were totally decreasing from 84.1 % to 52.0 %. Although they declined through the estuary, they were still dominant in this region. The percentage of C320 and C290 were all increasing from the river to the open lake water.

# Discussion
## PARAFAC-derived EEM components
This is the first time one sample FlFFF-EEM-PARAFAC technique was applied in an ecosystem continuum. Considering that this is a newly developed method, many questions were raised during applications that need to be concerned. For example, what is the difference between one sample FlFFF-EEM-PARAFAC and all subsamples involved PARAFAC? To distinguish the differences, all fractional subsample EEMs from all these six stations were assembled into one dataset and applied a conventional PARAFAC analysis. The final half-split validated model had four components, which were found no difference with those components identified from individual samples (TCC >0.95). Thus, the Component 1 to Component 4 in this model were also named as C475, C320, C290 and C410. However, the Fmaxs in each station were different with those derived from one-sample PARAFAC.
Unlike the conservative mixing behaviors of both humic-like components (C475 and C410) from one sample FlFFF-EEM-PARAFAC, ∑Fmax of them were deviated from conservative mixing line (Figure S6 (a)). No significant linear correlation between specific conductivity and the ∑Fmax of C475 (n=6, r = 0.72, p=0.11) and C410 (n=6, r=0.50, p=0.31) was observed. In terms of the relative fluorescence intensity, the relative humic-like C475 decreased along the transect, and two protein-like components (C320 and C290) relatively increased with decreasing specific conductivity (Figure S7 (b)). The relative intensity of C410, recognized as a microbial derived fluorescent component, remained unchanged along the transect. 
Since the Fox Rive plume is a natural ecological continuum, everything herein should change gradually and consistently. Thus, we believed that results from one sample FlFFF-EEM-PARAFAC are more reliable than all subsample PARAFAC regarding to ∑Fmax or relative fluorescence intensities. 
To better compare and interpret these fluorescent components, we separated them into three categories based on their biological lability: refractory, semi-labile and aquagenic. Although it has been reported that Peak A and Peak C have high photo-chemical reactivities (especially Peak C, impacted by predominant UVA in solar irradiation), C475, containing majorly Peak A and Peak C, has been proven as a biological refractory component (Murphy et al. 2018a). C290 and C320, specifically tyrosine-like and tryptophan-like component, are sorted into the aquagenic categories. C410, as described above, is categorized as a semi-labile component. Figure 7 (a) shows the relative importance of the three categories. Aquagenic DOM increased along the estuary, while the semi-labile DOM disappear gradually, and the refractory DOM remained consistently. If components from all subsample PARAFAC are sorted into these three categories, the relative importance of them are shown in Figure 7 (b). The refractory DOM decreased along the river plume while the semi-labile DOM were unvaried, which makes no sense. These results, on the other hand, further shows the advantages of the one sample FlFFF-EEM-PARAFAC.

## Size distribution and composition of DOM in the negative estuary
In comparison with a normal coastal estuary, our observations showed that the molecular size of DOM in the negative estuary is more consistent. The reasons for homogeneity of DOM size in a negative estuary, at least at Fox River – Green Bay estuary, are discussed below.
First, based on DLVO theory, diminish of ion density in ambient environment would thicken the electric double layer, and vice versa (Markus et al. 2016; Xu et al. 2018c). The decrease of DOM molecular size had been observed in marine estuaries by several field studies (Wells 2004; Lin et al. 2016a). However, the gradient of ion density in the negative estuary is relatively insignificant in this small spatial scale compared with salinity boost in a normal coastal estuary; the specific conductivity here declines from 463.4 μS/cm to 321.8 μS/cm, which is nearly 100 times less than the specific conductivity rise in normal estuaries (e.g. from 500 μS/cm to 50,000 μS/cm). Second, negligible flocculation, aggregation was observed. Despite the UV254 and Fluor350/450 (humic-like) of different size fractions decreased linearly, the relative each size fraction intensity remained constant (Figure 3). Meanwhile, the suspended particulate matter (SPM) was conservative mixed through the estuary, which implies that no addition or removal was found in this transportation (Table 1). Last but not the least, although the size distribution of DOM was partially impacted by pH (Romera-Castillo et al. 2014), the pH value, ranged from 8.7 to 9.1 in this negative estuary, was relatively constant, resulting in little impact on DOM molecular size (Table 1).
As for the DOM composition in the negative estuary, one sample FlFFF-EEM-PARAFAC method unveils the compositional structure change of fluorescent DOM. Although the fluorescent DOM is only a fraction of DOM, it potentially reflects the change of bulk DOM pool. Previous studies have proved that ion strength have in aquatic environments slight impact on the optical properties of CDOM (Del Castillo et al. 2000; Guo et al. 2007). Thus, this DOM composition variations were mostly due to the various sources and sinks of natural DOM.  

## Self-assembly supramolecular hypothesis 
Humic substances are regarded as a mixture of many molecules. Some soil scientists proposed that the structure of natural humic substance are supramolecular associations of relatively small heterogenous molecules held by weak dispersive forces such as van der Waals force and hydrogen bonds. Since its introduction, evidence supporting this hypothesis from several different analytical tools has been published. Romera-Castillo et al. found the size spectra from high performance size exclusion chromatography (HPSEC) were overlapped significantly between different fluorescence components (Romera-Castillo et al. 2014). It indicates the inclusion of fluorophores in different supramolecular assemblies. However, they manipulated their size fractionated EEM spectra by fitting them into a PARAFAC model generated using natural water samples from the National Park Everglade freshwater ecosystem. It would potentially miss some characteristic EEM signals and have additional artifacts during fitting processes since the PARAFAC model is not the optimization for the size fractionated EEM spectra. Another study confirmed the hypothesis using a HPSEC-PARAFAC2 technique, but unfortunately they don’t provide the online fluorescent DOM spectra (Wünsch et al. 2017). Here, the one sample FlFFF-EEM-PARAFAC results contributed an additional and robust evidence for the confirmation of the self-assembly supramolecular hypothesis. Figure 8 shows size spectra of two humic-like components (C475 and C410) in all six stations. They were accumulated and highly overlapped at 1-10 kDa size interval despite of their different sources. They are most likely represent small heterogeneous humic-like moieties associated to form the supramolecular assemblies. Thus, similar to the overlaps found in previous studies, our results provide a reliable support for the supramolecular assemblies hypothesis (Her et al. 2003; Boehme and Wells 2006; Romera-Castillo et al. 2014; Wünsch et al. 2017).

# Acknowledgement

