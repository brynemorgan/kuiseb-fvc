# Kuiseb–FVC
This repository contains data for spatiotemporal analysis of fractional vegetation cover (FVC) change along the Kuiseb River in the Namib Desert, reported in Morgan et al. (in prep.). Due to the size of the geospatial data, only the Landsat NDVI and FVC images are included here; extracted data from the unmanned aerial vehicle (UAV) orthophotos used to generate the Landsat FVC time series are included in table format.

## Authors

Bryn E. Morgan, Jonathan W. Chipman, Douglas T. Bolger, James T. Dietrich

Contact: bryn.morgan@geog.ucsb.edu

## Citation

Morgan, B. E., Chipman, J. W., Bolger, D. T., & Dietrich, J. T.  (2020). Spatiotemporal analysis of vegetation cover change in a large ephemeral river: multi-sensor fusion of unmanned aerial vehicle (UAV) and Landsat imagery. Manuscript in review.


## Data

Tables are included in .xls format as described below.



<span style="font-size:10pt">

| Folder | File names | Description |
|-----------|-----------------------------------------------|----------------------------------------------------------------------|
| [data/Landsat_2016_VI_Tables](data/Landsat_2016_VI_Tables) | Site_#a_VI.xls (# corresponds to the flight number) | Vegetation index (EVI, MSAVI, NDVI, VARI, VIG/GRVI) data derived from a Landsat Surface Reflectance image obtained 31 July 2016 for UAV missions. |
| [data/Landsat_FVC_Tables](data/Landsat_FVC_Tables) | L#_DD-MMM-YY_Mod_Cover.xls (# refers to the Landsat sensor) | Modeled FVC for the given image date extracted in 500-m segments along the river from [Landsat FVC images](images/Landsat_FVC) |
| [data/Landsat_NDVI_Tables](data/Landsat_NDVI_Tables) | L#_DD-MMM-YY_Mod_NDVI.xls (# refers to the Landsat sensor) | NDVI for the given image date extracted in 500-m segments along the river from [Landsat NDVI images](images/Landsat_NDVI) |
| [data/River_Segments_500m_Labeled.shp](data/River_Segments_500m_Labeled.shp) | | Riparian zone polygon divided into contiguous 500-m segments, labeled in the "POLY" field from upstream to downstream |
| [data/UAV_FVC_Tables](data/UAV_FVC_Tables) | Site_#a_Cover.xls (# corresponds to the flight number) | FVC extracted from UAV data by Landsat pixel. Used with the [Landsat 2016 VI tables](data/Landsat_2016_VI_Tables) to generate the models in Figs. 6 and 7. |

</span>


## Images

The raw UAV images and orthoimages from each step of the UAV workflow described in Fig. 2 for an example site (Alpha) are available in an accompanying Zenodo repository, [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4328408.svg)](https://doi.org/10.5281/zenodo.4328408). Agisoft processing reports for the RGB and NIR orthoimages for the two missions at this site can be found in the [processing](processing) folder.

Landsat NDVI and FVC time series generated from the FVC model (Eq. 7) are included in the [images](images) folder as described in the table below.



<span style="font-size:10pt">

| Folder | File names | Description |
|-----------|-----------------------------------------------|----------------------------------------------------------------------|
| [images/Landsat_FVC](images/Landsat_FVC) | L#_DD-MMM-YY_Mod_Cover.img (# corresponds to the flight number) | Landsat-derived FVC time series, 1984-2019. |
| [images/Landsat_NDVI](images/Landsat_NDVI) | L#_DD-MMM-YY_Mod_NDVI.img (# corresponds to the flight number) | Landsat-derived NDVI time series, 1984-2019. |

</span>



## License

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.