# EMIT-Data-Resources

Welcome to the EMIT-Data-Resources repository. This repository provides guides, short how-tos, and tutorials to help users access and work with data from the Earth Surface Mineral Dust Source Investigation (EMIT) mission. In the interest of open science this repository has been made public but is still under active development. All jupyter notebooks and scripts should be functional, however, changes or additions may be made. Contributions from all parties are welcome.

> Please note that EMIT data files are large and orthorectification expands their size. If using an Openscapes 2i2c JupyterLab instance please select a Large size server.

---

## Fridays in February 2023 Upcoming Workshop Series!

Please join us February 3, 10, and 17th from 1:00 - 3:00pm EST. to learn about working with EMIT radiance and relfectance products. Sign up for the workshop [here](https://tinyurl.com/2tp3cx3t).

---

## EMIT Background  

The [EMIT](https://earth.jpl.nasa.gov/emit/) Project delivers space-based measurements of surface mineralogy of the Earth’s arid dust source regions. These measurements are used to initialize the compositional makeup of dust sources in Earth System Models (ESMs). The dust cycle, which describe the generation, lofting, transport, and deposition of mineral dust, plays an important role in ESMs.  Dust composition is presently the largest uncertainty factor in quantifying the magnitude of aerosol direct radiative forcing.  By understanding the composition of mineral dust sources, EMIT aims to constrain the sign and magnitude of dust-related radiative forcing at regional and global scales. During its one-year mission on the International Space Station (ISS), EMIT will make measurements over the sunlit Earth’s dust source regions that fall within ±52° latitude. EMIT will schedule up to five visits (three on average) of each arid target region and only acquisitions not dominated by cloud cover will be downlinked. EMIT-based maps of the relative abundance of source minerals will advance the understanding of the current and future impacts of mineral dust in the Earth system.  

EMIT Data Products are distributed by the [LP DAAC](https://lpdaac.usgs.gov/). Learn more about EMIT data products from [EMIT Product Pages](https://lpdaac.usgs.gov/product_search/?query=emit&status=Operational&view=cards&sort=title) and search for and download EMIT data products using [NASA EarthData Search](https://search.earthdata.nasa.gov/search?q=%22EMIT%22)

---

## Prerequisites/Setup Instructions

This repository requires that users set up a compatible Python environment and download the EMIT granules used. See the `setup_instuctions.md` file in the `./setup/` folder.

## Repository Contents  

Content in this repository is divided into 3 categories:  

### **1. Guides**  

Web viewable Resources in markdown format that walk through a task:  

+ Getting EMIT Data using EarthData Search - A thourough walkthrough for using [EarthData Search](https://search.earthdata.nasa.gov/search) to find and download EMIT data.

### **2. How-To Notebooks**

Short jupyter notebooks that explain how to complete a task:  

+ How to Convert to ENVI Format - Convert from downloaded netCDF4 (.nc) format to .envi format.
+ How to Orthorectify - Use the geometry lookup table (GLT) included with the EMIT netCDF4 file to project on a geospatial grid (EPSG:4326).
+ How to Extract Point Data  - Extract spectra using lat/lon coordinates from a .csv and build a dataframe/.csv output.
+ How to Extract Area Data - Clip to/extract an area defined by a .geojson or shapefile.
+ How to use EMIT Quality Data - Build a mask using bands from  an EMIT L2A Mask file and apply it to an L2A Reflectance file.

### **3. Tutorial Notebooks**  

Longer jupyter notebooks that walk through a process or concept:  

+ 01 Exploring EMIT L2A Reflectance  

---

## Helpful Links  

+ [JPL EMIT Website](https://earth.jpl.nasa.gov/emit/)  

+ [EMIT Github Repository](https://github.com/emit-sds) - Main EMIT Repository  

+ [EMIT Utilities Github Repository](https://github.com/emit-sds/emit-utils) - General convenience utilities for working with EMIT data

+ [L2A Reflectance User Guide](https://lpdaac.usgs.gov/documents/1569/EMITL2ARFL_User_Guide_v1.pdf)  

+ [L2A Algorithm Theoretical Basis Document](https://lpdaac.usgs.gov/documents/1571/EMITL2A_ATBD_v1.pdf)  

+ [EMIT LP DAAC Product Pages](https://lpdaac.usgs.gov/product_search/?query=emit&status=Operational&view=cards&sort=title) - Learn more about available EMIT products  

+ [EMIT on Earth Data Search](https://search.earthdata.nasa.gov/search?q=%22EMIT%22) - Find EMIT Data  

---

## Contact Info:  

Email: LPDAAC@usgs.gov  
Voice: +1-866-573-3222  
Organization: Land Processes Distributed Active Archive Center (LP DAAC)¹  
Website: <https://lpdaac.usgs.gov/>  
Date last modified: 01-20-2023  

¹Work performed under USGS contract G15PD00467 for NASA contract NNG14HH33I.  
