# EDS 220 Homework 4 - Visualizing fire scars through false color

This repository hosts all the work completed by Amapola Garcia during the discussion sections of EDS 220 - *Working with Environmental Datasets*.

* **Author:** Amapola Garcia
* **Date:** November 15,2026
* **Course Title:** [EDS 220 - Working with Environmental Datasets](https://bren.ucsb.edu/courses/eds-220)
* **Program:** [UCSB Master of Environmental Data Science](https://bren.ucsb.edu/masters-programs/master-environmental-data-science).
* **Term:** Fall 2026

Teaching Team:
- **Instructor:** [Carmen Galaz García](https://github.com/carmengg)
- **Teaching Assistant:** [Fatiq Nadeem](https://github.com/fatiqnadeem) 

## About
In February 2021, a severe winter storm swept across the U.S. central plains, setting national records for low temperatures. Texas was especially affected, with widespread electricity and water outages. This event ranks among the most severe winter weather incidents in history, resulting in loss of life and long-term economic consequences. In the aftermath, political debate and blame can obscure the facts.

**This repository contains my work for EDS 220 Homework 4. The notebook uses Landsat 8 imagery and fire perimeter data to create true-color and false-color images of the Eaton and Palisades fires, then maps the fire perimeters over the false-color image.** 

## Highlights of the Analysis
- Explored fire perimeter data and CRS information.
- Restored the CRS information for the Landsat dataset.
- Created true-color and false-color Landsat images.
- Mapped both fire perimeters over the false-color image.

## Instructions
I will be creating a false color image of the Eaton and Palisades Fires using remote sensing data, highlighting the fire scar and exploring how coding and data visualization support enviormental monitoring.

## Data
**Landsat imagery:Landsat Collection 2 Level-2 atmospherically:**
Collection of bands (**red,green,blue,near-infrared and shortwave infared**)is available in the EDS 220 course shared data folder. It contains Landsat 8 surface reflectance bands and was retrieved from the [Microsoft Planetary Computer](https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2).

- `landsat8-2025-02-23-palisades-eaton.nc`
  
**Fire perimeters for the Eaton and Palisades fires:** 
The Eaton and Palisades fire perimeters were downloaded from [Los Angeles County Enterprise GIS](https://egis-lacounty.hub.arcgis.com/maps/ad51845ea5fb4eb483bc2a7c38b2370c/about) as separate shapefile datasets.

*More than one File*
  - `Eaton_Perimeter_20250121`
  - `Palisades_Perimieter_20250121`

##  Repository Structure
```bash

eds220-hwk4
├──  README.md
├── hwk4-task2-false-color-Garcia.ipynb #Jypter notebook for the analysis
├── .gitignore                    
│    data/                        
|     ├── landsat8-2025-02-23-palisades-eaton.nc
|     ├── Eaton_Perimeter_20250121
│     └── Palisades_Perimieter_20250121         
└── LICENSE
```

## References
Los Angeles County Enterprise GIS. (2025). *Palisades and Eaton dissolved fire perimeters (2025)* [GIS data]. https://egis-lacounty.hub.arcgis.com/maps/ad51845ea5fb4eb483bc2a7c38b2370c/about

Microsoft Planetary Computer. (n.d.). *Landsat Collection 2 Level-2* [Data catalog]. https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2

M. M. Bennett, J. K. Chen, L. F. Alvarez León, and C. J. Gleason, “The politics of pixels: A review and agenda for critical remote sensing,” Progress in Human Geography, vol. 46, no. 3, pp. 729–752, June 2022, doi: 10.1177/03091325221074691. Available: https://journals.sagepub.com/doi/10.1177/03091325221074691. [Accessed: Nov. 14, 2024]

MEDS/EDS 220. (n.d.). *Assignment 4: Visualizing fire scars through false color*. https://meds-eds-220.github.io/MEDS-eds-220-course/assignments/assignment4-palisades-eaton-fires.html