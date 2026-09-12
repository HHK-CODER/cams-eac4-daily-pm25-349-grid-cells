\# Daily CAMS EAC4 PM2.5 for 349 Unique Grid Cells, 2019–2024



This repository provides daily surface PM2.5 concentrations derived from the \*\*Copernicus Atmosphere Monitoring Service (CAMS) Global Reanalysis of Atmospheric Composition (EAC4)\*\* for 349 spatially unique matched CAMS grid cells from 1 January 2019 to 31 December 2024.



\## Dataset



\*\*File:\*\* `cams\_eac4\_daily\_pm25\_ug\_m3\_2019\_2024\_349\_unique\_grid\_cells.csv`



The dataset contains daily PM2.5 concentrations in \*\*µg/m³\*\*. Each retained city-centroid label maps to one unique nearest CAMS EAC4 grid cell. City centroids that mapped to the same CAMS cell were excluded so that identical PM2.5 target series were not treated as independent spatial observations.



\## Data fields



The principal fields are:



| Field | Description |

|---|---|

| `date` | UTC date of the daily aggregation |

| `cohort\_city\_id` | Stable identifier for the selected representative location |

| `cams\_eac4\_pm25\_ug\_m3` | Daily mean PM2.5 concentration in µg/m³ |

| `country`, `city`, `country\_iso2` | Representative location labels |

| `input\_city\_latitude`, `input\_city\_longitude` | City-centroid coordinates used for matching |

| `matched\_cams\_grid\_latitude`, `matched\_cams\_grid\_longitude\_degrees\_east` | Matched CAMS EAC4 grid-cell coordinates |

| `nearest\_grid\_distance\_km` | Distance between the selected centroid and matched grid cell |

| `daily\_coverage\_pct` | Percentage of expected three-hourly fields contributing to the daily mean |

| `daily\_record\_status` | Daily completeness status |



\## Source and processing



The source product is the \*\*CAMS Global Reanalysis of Atmospheric Composition (EAC4)\*\*, accessed through the Copernicus Atmosphere Data Store. The dataset uses the EAC4 `particulate\_matter\_2.5um` variable. Native concentrations in kg/m³ were converted to µg/m³ by multiplying by 1,000,000,000. Each daily value is the arithmetic mean of eight three-hourly UTC fields.



The source data are reanalysis estimates rather than station observations. Accordingly, this dataset should not be interpreted as a global in situ monitoring database.



\## Citation



If you use this derived dataset, please cite this repository, the associated study, and the CAMS EAC4 source:



> Inness, A., et al. (2019). The CAMS reanalysis of atmospheric composition. \*Atmospheric Chemistry and Physics, 19\*, 3515–3556. https://doi.org/10.5194/acp-19-3515-2019



\## License and attribution



This repository is released under the \*\*Creative Commons Attribution 4.0 International License (CC BY 4.0 )\*\*. Users must provide attribution to this repository and acknowledge the Copernicus/CAMS source data.



Copernicus and CAMS data are provided under the Copernicus licence to use Copernicus products. Users remain responsible for complying with all applicable source-data terms.



