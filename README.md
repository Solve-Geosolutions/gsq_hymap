![Datarock](assets/datarock_logo_2_rect.jpeg)

# Queensland HyMap Data Sets

This repository contains code and workflows used to demonstrate open source approaches to processing and manipulating hyperspectral data sets acquired by HyVista Corporation's HyMap system. The data was acquired in 2006-2008 as part of the Next Generation Mineral Mapping initiative, a collaborative project run by the CSIRO, the Geological Survey of Queensland, Geoscience Australia and James Cook University to collect and analyse airborne hyperspectral and satellite borne multispectral data in prospective areas of North Queensland.

## Code

The *code* directory contains the following notebooks:

 1. **01_apply_geocorrections_and_mosaic.ipynb** - a notebook that reads geometry lookup tables and reflectance data from individual flight swaths to create a hyperspectral mosaic in ENVI grid format.
 2. **02_vegetation_identification.ipynb** - a notebook that reads the mosaic ENVI grid to calculate an NDVI product using a memory efficient blockwindow workflow.
 3. **03_convex_hull_computation.ipynb** - a notebook that applies a convex hull continuum removal workflow to reflectance data and outputs a continuum removed ENVI grid.
 4. **04_white_mica_abundance.ipynb** - a crude attempt at calculating white mica abundance from the convex hull continuum removed ENVI grid.


## Requirements



## Data

The Geological Survey of Queensland hosts a number of products from the HyMap surveys which can be downloaded [**here**](https://geoscience.data.qld.gov.au/data/dataset/?type=spectral). The raw data used in this repository requires temporary AWS access links and the reader is advised to contact the [**GSQ**](https://www.resources.qld.gov.au/?contact=gsq) for this. 
