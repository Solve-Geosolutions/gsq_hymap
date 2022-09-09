![Datarock](assets/datarock_logo_2_rect.jpeg)

# Queensland HyMap Data Sets

This repository is complimentary to a Datarock applied science [blogpost](link_to_blogpost) 

 contains code and workflows used to demonstrate open source approaches to processing and manipulating hyperspectral data sets acquired by HyVista Corporation's HyMap system. The data was acquired in 2006-2008 as part of the Next Generation Mineral Mapping initiative, a collaborative project run by the CSIRO, the Geological Survey of Queensland, Geoscience Australia and James Cook University to collect and analyse airborne hyperspectral and satellite borne multispectral data in prospective areas of North Queensland.

## Code

The *code* directory contains the following notebooks:

###  **01_apply_geocorrections_and_mosaic.ipynb**

This notebok was used to apply geometry lookup tables to raw reflectance data cubes in order to generate a georeferenced hyperspectral mosaic in ENVI grid format.

![01_convex_hull_computation.ipynb](assets/notebook_1_image.png)

###  **02_vegetation_identification.ipynb**

A notebook used to derive normalised difference vegetation index and a crude vegetation mask from the georeferenced hyperspectral mosaic. A memory efficient native ENVI blockwindow approach was used for computation.

![02_convex_hull_computation.ipynb](assets/notebook_2_image.png)

### **03_convex_hull_computation.ipynb**

A notebook used to apply a slow, pixel-wise convex hull continuum removal to the hyperspectral data. 

![03_convex_hull_computation.ipynb](assets/notebook_3_image.png)


### **04_white_mica_abundance.ipynb**

A simplistic white mica feature depth and feature position extraction workflow using quadratic functions fitted to a feature window.

![04_convex_hull_computation.ipynb](assets/notebook_4_image.png)

## Data

The Geological Survey of Queensland hosts a number of products from the HyMap surveys which can be downloaded [**here**](https://geoscience.data.qld.gov.au/data/dataset/?type=spectral). The raw data used in this repository requires temporary AWS access for which that reader is advised to contact [**GSQ**](https://www.resources.qld.gov.au/?contact=gsq) directly. 

