# Description
This repository contains scripts processing East Antarctic ecosystem features and returns the likely distinct bioregions through clusterings

# Usage
A virtual environment is needed to run the dependencies.

## Run on Galaxy
If you plan on running the script on Galaxy.eu, you can use Jupyter Notebook Interactive tool.*

\* A Galaxy account is required to use the tool

## Run on local or another 
You can use `environment.yml`to create the proper environment.

# Required packages
* r-r.utils 
* r-tidyverse 
* libgdal-hdf5 
* r-ggplot2
* r-rcpp 
* openssl 
* r-sf 
* r-terra 
* r-ncdf4
* r-lubridate
* r-rcolorbrewer 
* r-lattice 
* r-png
* r-raster
* r-fnn
* r-cluster 
* r-remotes 
* r-devtools

```bash
conda create --file environment.yml
```

[![R.utils license](https://img.shields.io/github/license/nextflow-io/nextflow.svg?colorB=58bd9f&style=popout)]()

## Retrieve Copernicus Data
### Ice Concentration
```bash
copernicusmarine subset --dataset-id osisaf_obs-si_glo_phy_sic-south_my_amsr_cdr_P1D-m --variable raw_ice_conc_values --variable ice_conc --start-datetime 2003-01-01T00:00:00 --end-datetime 2010-12-31T00:00:00 --minimum-longitude 30 --maximum-longitude 150 --minimum-latitude -70 --maximum-latitude -60 
```