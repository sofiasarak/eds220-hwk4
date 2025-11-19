# EDS220 Homework 4: LA County Fires, January 2025

This repository contains the response to Homework 4 in EDS220 - *Working with Environmental Datasets*, completed by Sofia Sarak.

These analyses primarly use remote sensing data to explore the impacts of the Eaton and Palisades wildfires in Los Angeles County. The two fires occurred nearly simultaneously and had  widespread impact, inflicting both ecological and infrastructural damage on the area. By using remote sensing data and assigning infrared bands to visible colors, we are able to highlight vegetation health, burn severity, and the extent of fire scars remnant after the fire. 

This notebook concludes with the creation of a false color image of the Eaton and Palisades Fires, highlighting the fire scar with an overlay of fire perimeters.

For more information on the homework assignment itself (including all of the data and sources), reference the [assignment description](https://meds-eds-220.github.io/MEDS-eds-220-course/assignments/assignment4-palisades.html).

## Data Sources

**Landsat/remote sensing:**

The dataset used in this analysis is a simplified collection of bands (red, green, blue, near-infrared and shortwave infrared) from the Landsat Collection 2 Level-2 atmospherically corrected surface reflectance data, collected by the Landsat 8 satellite. Landsat data is provided by a series of Earth-observing satellites jointly managed by NASA and the U.S. Geological Survey (USGS), and stores a significant amount of reflectance information about the Earth's surface.

The data was retrieved from the [Microsoft Planetary Computer data catalogue](https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2) catalogue and clipped to an area surrounding the fire perimeters by the [EDS220](https://meds-eds-220.github.io/MEDS-eds-220-course/) course team.

Accessed November 15, 2025.

**Palisades and Eaton fire perimeter:**

Palisades and Eaton fire perimeter data were sourced from [LA County's GIS hub](https://egis-lacounty.hub.arcgis.com/maps/ad51845ea5fb4eb483bc2a7c38b2370c/about). It contains dissolved fire boundaries for Eaton and Palisades fires. It is a public data set, published January 21, 2025 and last updated on February 26, 2025

Accessed November 15, 2025.

#### References

**Data:**

Earth Resources Observation and Science (EROS) Center. (2020). Landsat 8–9 Operational Land Imager / Thermal Infrared Sensor Level-2, Collection 2 [Dataset]. U.S. Geological Survey. https://doi.org/10.5066/P9OGBGM6

Los Angeles County Enterprise GIS. (2025). Palisades and Eaton Dissolved Fire Perimeters [Dataset]. Los Angeles County. https://egis-lacounty.hub.arcgis.com/maps/ad51845ea5fb4eb483bc2a7c38b2370c/about

**Education Resources (used for understanding):**
- [Band designations for the Landsat satellites (USGS)](https://www.usgs.gov/faqs/what-are-band-designations-landsat-satellites)
- [Common Landsat Band Combinations (USGS)](https://www.usgs.gov/media/images/common-landsat-band-combinations)
- [How to Interpret a False-Color Satellite Image (NASA)](https://earthobservatory.nasa.gov/features/FalseColor)
- [True Color Imagery (NOAA)](https://coastwatch.noaa.gov/cwn/product-families/true-color-imagery.html)
- 

## Repository Structure
```
├── data
│   ├── Eaton_Perimeter_20250121
│   │   ├── Eaton_Perimeter_20250121.cpg
│   │   ├── Eaton_Perimeter_20250121.dbf
│   │   ├── Eaton_Perimeter_20250121.prj
│   │   ├── Eaton_Perimeter_20250121.shp
│   │   └── Eaton_Perimeter_20250121.shx
│   ├── landsat8-2025-02-23-palisades-eaton.nc
│   └── Palisades_Perimeter_20250121
│       ├── Palisades_Perimeter_20250121.cpg
│       ├── Palisades_Perimeter_20250121.dbf
│       ├── Palisades_Perimeter_20250121.prj
│       ├── Palisades_Perimeter_20250121.shp
│       └── Palisades_Perimeter_20250121.shx
├── hwk4-task2-false-color-SARAK.ipynb
└── README.md

```
## Course Information

-   **Course Title:** [EDS 220 - Working with Environmental Datasets](https://meds-eds-220.github.io/MEDS-eds-220-course/)
-   **Term:** Fall 2025
-   **Program:** [UCSB Masters in Environmental Data Science](https://bren.ucsb.edu/masters-programs/master-environmental-data-science).

Teaching Team:

-   **Instructor:** [Carmen Galaz García](https://github.com/carmengg)
-   **Teaching Assistant:** [Annie Adams](https://github.com/annieradams)

Complete materials for the discussion sections and additional resources can be found on the [course website](https://meds-eds-220.github.io/MEDS-eds-220-course/).

*This README was adapted from the README template provided in EDS220; see course details and original repository [here](https://github.com/sofiasarak/eds220-2025-in-class).*

