---
layout: post
date: 2017-07-05 16:52
categories: Research
title: PARAFAC Abnormality solution
---
PARAFAC Analysis results from Stephen et al., 2016 (STE)
![](\image\PARAFAC_EEM_Correction\Stephen 2016 STE.jpg)
PARAFAC Analysis results from Zhou et al., 2016 (JGLR)
![](\image\PARAFAC_EEM_Correction\Xu 2016 WR.jpg)
PARAFAC Analysis results from Xu and Guo., 2016 (WR)
![](\image\PARAFAC_EEM_Correction\Zhou 2016 JGLR.jpg)

Abnormality: abrupt decline of some peaks

![](\image\PARAFAC_EEM_Correction\Stephen-2016-STE.jpg)
![](\image\PARAFAC_EEM_Correction\Xu-2016-WR.jpg)
![](\image\PARAFAC_EEM_Correction\Zhou-2016-JGLR.jpg)

## Compared with literatures

### Walker et al. 2013
![](\image\PARAFAC_EEM_Correction\Walker et al. 2013.jpg)

### Stedmon & Markager 2005
![](\image\PARAFAC_EEM_Correction\Stedmon&Markager 2005.jpg)

### Stedmon et al 2003
![](\image\PARAFAC_EEM_Correction\Stedmon et al 2003.jpg)

Hypothesis: Cut EEMs improperly

```
FirstOrderCut = [-40 15];
SecondOrderCut = [-40 15];
InsertedData = [NaN 0];
for i = 1:2
    if FirstOrderCut(i) ~= NaN
        for j = 1: length(Ex)
            k = find (Em<Ex(j)-FirstOrderCut(i));
            X(:,k,j) = InsertedData(i);
        end
    end
    if SecondOrderCut (i) ~= NaN
        for j = 1:length(Ex)
            k = find (Em>Ex(j)*2.05+SecondOrderCut(i));
            X(:,k,j) = InsertedData(i);
        end
    end
end
```
Demostration:
![](\image\PARAFAC_EEM_Correction\LM01-02m-09182015-Retentate-Bulk-Dilution10.jpg)

Solution:
```
InsertedData = [NaN NaN]
```
Results:
## Introduction of samples

### Samples:

Yukon River downstream

### Sampling time:

2004-2005

### Sample categories:

colloidal organic matter (>1kDa), low molecular weight organic matter (<1kDa), dissolved organic matter (<0.45e-6 m)

### Before program revised:

3 components decomposed by PARAFAC program:

![](\image\PARAFAC_EEM_Correction\Fluorescence-EEM-Plot-of-component-123.jpg)

4 components from PARAFAC:

![](\image\PARAFAC_EEM_Correction\Fluorescence-EEM-Plot-of-component-1234.jpg)

### After revised:

3 components decomposed by PARAFAC program:

![](\image\PARAFAC_EEM_Correction\Fluorescence-EEM-Plot-of-component-123-revised.jpg)

4 components from PARAFAC:

![](\image\PARAFAC_EEM_Correction\Fluorescence-EEM-Plot-of-component-1234-revised.jpg)

### Comparison

| ﻿Component   | before program revised |               | After revised   |               |
|-------------|------------------------|---------------|--------------------|---------------|
|             | Excitation (nm)        | Emission (nm) | Excitation (nm) | Emission (nm) |
| 3Components                          |               |                 |               |
| C1          | 280                    | 485           | 260             | 480           |
| C2          | 250                    | 480           | 250             | 420           |
| C3          | 220                    | 405           | <250            | 330           |
| 4Components                          |               |                 |               |
| C1          | 230                    | 450           | 250             | 420           |
| C2          | 310                    | 410           | 270             | 500           |
| C3          | 385                    | 480           | 260/375         | 480           |
| C4          | <220                   | 380           | <250            | 330           |
