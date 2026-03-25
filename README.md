# README: Data Extraction and Calculation for Ad Valorem Tariffs Rates and Forest Growing Stock and Forest Stock Growth for TiMBA 


## Overview

This dataset serves as a guide for understanding how the ad valorem tariffs used in TiMBA - a partial economic equilibrium model for the global forest products market were generated and updated based on the WTO's tariff data. Further, this dataset contains information on forest growing stock and forest stock growth for 180 countries, as considered in the TiMBA model. The data are essential for modelling scenarios on forest development and trade flows.
By following the explanations outlined in the respective manual (Scenario_input_data_generation_Tariffs_Forest), we ensure transparency, accuracy and consistency in mean ad valorem tariff calculations as well as forest growing stock data and annual changes across the products and countries listed. For any further details, the tariff and forest data can be accessed directly through the provided database sources.
Data are provided in two tables: (1) AdValoremRates.csv and (2) ForestGrowingStock

## Data Sources

This repository uses data from multiple FAO sources.

Source:

### FAOSTAT

FAO. FAOSTAT Statistical Database.
https://www.fao.org/faostat/

### Attribution

© FAO (FAOSTAT and FRA 2025)

### Global Forest Resources Assessment (FRA 2025)

FAO. Global Forest Resources Assessment 2025.
https://fra-data.fao.org/assessments/fra/2025

### License:
FAOSTAT data are licensed under the Creative Commons Attribution 4.0 International (CC BY 4.0):
https://creativecommons.org/licenses/by/4.0/

### Data Processing

The original FAOSTAT data have been modified for the purposes of this project.
Modifications include:

- restructuring of tables
- renaming of variables
- filtering and aggregation
- formatting changes

These modifications do not affect the original licensing of the data.

### Licensing
Code in this repository is licensed under the GNU GPL v3 License (see LICENSE)
FAOSTAT data (raw and processed) remain subject to the CC BY 4.0 license (see DATA_LICENSE.md)

No additional restrictions are imposed on the original FAOSTAT data.
