## Advisory

The original project was used on a private, Illinois Data Science Club (IDSC) GitHub repository that I am unable to make public. Instead, I am in the process of transferring over key files and data. The project was presented at the IDSC Data Dive of Fall 2025, and placed in the top 10.

## Project Overview

This project analyzes coral reef data to better understand the patterns and drivers of coral bleaching. Coral reefs are critical ecosystems that support immense biodiversity, protect coastlines, and sustain global fisheries and tourism. However, rising ocean temperatures and other environmental stressors are causing widespread bleaching, threatening both natural ecosystems and human economies.

The goal of this project is to identify environmental factors associated with bleaching events and explore how these events vary across regions. By analyzing this data, we hope to gain insights that can inform conservation strategies, predict high-risk periods for reefs, and assess the broader ecological and economic impacts of reef degradation.

## Data Description

The dataset used in this project tracks coral reef health and environmental conditions across multiple sites worldwide. Data was collected from field surveys and satellite monitoring programs, recording both biological and environmental metrics.

Data sources: The Biological and Chemical Oceanography Data Management Office (BCO-DMO) - doi: 10.1038/s41597-022-01121-y

Time period covered: 1980–2020

Size of dataset: Approximately 41,000 observations with 62 columns

### Key Variables
| Variable Name     | Description                          | Data Type   | Units/Format | Notes                                             |
| :---------------- | :----------------------------------- | :---------- | :----------- | :------------------------------------------------ |
| `Realm_Name`         | Marine Ecoregions of the World (MEOW) Spalding et al. 2007 | String      | N/A          | Region   |
| `Latitude_Degrees`   | Latitude Coordinates         | Float       | Degrees      | Positive = North, Negative = South                        |
| `Longitude_Degrees`  | Longitude Coordinates        | Float       | Degrees      | Positive = East, Negative = West                          |
| `Date`               | Date of observation                  | Date        | YYYY-MM-DD   |              |
| `SSTA`               | Sea surface temperature Anomaly              | Float       | °C           | Weekly SST minus weekly climatological SST |
| `TSA`   | Thermal Stress Anomaly         | Float       | °C      | Weekly sea surface temperature minus the maximum of weekly climatological sea surface temperature                        |
| `ClimSST`   | Climatological sea surface temperature (SST)        | Float       | °C      |  Based on weekly SSTs for the study time frame, created using a harmonics approach                      |
| `Percent_Bleaching`  | An average of four transect segments (Reef Check) or average of a bleaching code       | Float       | %            |         |
| `Percent_Cover`      | Average cover value (percent) | Float | %         | 
| `Distance_to_Shore`   | The distance of the sampling site from the nearest land         | Float       | Meters      |                         |
| `Depth_m`   | depth of sampling site        | Float       | Meters      |                         |
