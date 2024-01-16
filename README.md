### Site Suitability Analysis for Solar PV Power Plants in Indonesia

* Please download htmls to view

#### Description:
* Based on an analysis of projected electricity demand, renewable electricity supply targets and existing, planned and under-construction renewable generation, Indonesia will require 27GW of installed solar PV power plants (PP) capacity by 2030.
* This analysis uses a spatial multi-criteria decision making (MCDM) analysis to recommend suitable sites for solar PP development in Indonesia.
* A financial analysis is conducted to recommend the projects.

#### Data:
* Built-settlements: WorldPop hub; University of Southampton; University of Louisville; Columbia University, 2018
* Protected and Sensitive Natural Areas: United Nations Environment Programme (UNEP-WCMC), 2013
* Land use: Climate Change Initiative (CCI), 2023
* Elevation: DIVA-GIS, SRTM 90m DEM Digital Elevation Database, 2023
* Slope: Derived from elevation using R programming
* Aspect: Derived from elevation using R programming
* Solar radiation (Surface Solar Radiation Downwards (SSRD)): Copernicus Climate Change Service (C3S) Climate Data Store(CDS). ‘ERA5-Land monthly averaged data from 1950 to present’, 2022
* Temperature (2m temperature): Copernicus Climate Change Service (C3S) Climate Data Store (CDS). ‘ERA5-Land monthly averaged data from 1950 to present’, 2022
* Roads: DIVA-GIS, Digital Chart of the World: Roads 2023
* Power infrastructure Open Street Map (OSM) (downloaded using R programming)

#### Method:
1. Create Restricted Layer - NO solar PPs in this area:
    * built-settlements, elevation > 90m, slope > 5 degrees, protected and sensitive natural areas, forests, cropland.
2. Create Suitability Layer - Rate areas most suitable for development using criteria:
    *  Proximity to existing power lines, main roads, and built settlements is considered favourable to reduce costs of added infrastructure
    *  Lower temperatures favoured over higher temperatures due to decreased efficiency of panels at high temperatures
    *  South-facing slopes favoured
    *  Higher, flatter areas below 90m favoured due to thinner atmosphere and ease of construction
3. Exclude restricted areas from Suitability Layer and reclassify
4. Site Selection - select top rated sites for required capacity
5. Financial Analysis
6. Recommend sites for development
