# **Fall 2025 Command-Line GIS Final Project**
## Housing Parcels Located in Flood Zones (Plainfield, NJ)

**Created by**: Nicholas Seu

**Course**: 34:970:595 - Command-Line GIS

## Overview:
* **Static Map #1**: Plainfield Parcels and Flood Zones
* **Static Map #2**: Plainfield Residential Parcels By Property Value Located in Flood Zones
* **Interactive Webmap**: A map that displays Plainfield's Residential Parcels by Their Property Value, Flood Zones, and adds a 15-Minute Walking Buffer from the Plainfield Train Station

# Static Map #1: Plainfield Parcels and Flood Zones

<img src="staticmap1.png" height="855" width="95%">

# Static Map #2: Plainfield Residential Property Values

<img src="staticmap2.png" height="855" width="95%">

# Interactive Webmap

This map includes:
* Residential Parcels in Plainfield by Sale Value
* Flood Zones (High Risk or Moderate to Low Risk) Categorized by FEMA Flood Codes
* 15-Minute Walking Buffer from Plainfield Train Station
List item


<iframe src="interactive_map.html" height="855" width="95%"></iframe>

You can explore this map [as its own webpage here](test.html)

# Data Description:
### Below is a list of sources that were used to create these maps:
**[FEMA's National Flood Hazard Layer (NFHL) Viewer ](https://www.arcgis.com/apps/webappviewer/index.html?id=8b0adb51996444d4879338b5529aa9cd)** - 
* Obtained From: ArcGIS.com
* Prepared By: FEMA
* Last Updated: December 16, 2021
* Original Format: Database Files and Plain Text Files
* Extra Steps Taken: Flood zones that were identified as 'AE', 'A', 'AO', 'AH' were grouped together as "High-Risk Areas" while the 'X' zones were grouped together as "Moderate to Low Risk Areas."
* Challenges: N/A

**[Union County MODIV Parcel Data](https://njogis-newjersey.opendata.arcgis.com/documents/79789530a56d425082afade9fea64252/about)** - 
* Obtained From: NJGIN
* Prepared By: New Jersey Office of GIS
* Last Updated: November 24, 2025 
* Original Format(s): Shapefiles and Database Files
* Extra Steps Taken: The parcel shapefile was merged with the Union County Tax List and was then clipped to Plainfield specifically, and then filtered to only show parcels that were identified as residential. Afterwards, all parcels belonging to the same municipality were dissolved into a single multi-polygon feature. Finally, the data found in the sale price column was specifically highlighted to show the value of the homes located in Plainfield.
* Challenges: Initially, it was challenging to figure out how to filter out all of the irrelevant data. Additionally, the dataset had a lot of columns, so it took some time to narrow it down to the ones I needed.

**[United States 2023 Census Tracts](https://data2.nhgis.org/options)** -
* Obtained From: NHGIS
* Prepared By: U.S. Census Bureau
* Last Updated: December 17, 2024
* Original Format: Shapefiles
* Extra Steps Taken: Converted the coordinate reference system from 102003 to 3424
* Challenges: N/A

**[Rail Stations of NJ Transit](https://njogis-newjersey.opendata.arcgis.com/datasets/NJTRANSIT::rail-stations-of-nj-transit/about)** -
* Obtained From: NJGIN
* Prepared By: NJ Transit GIS Department
* Last Updated: July  21, 2021
* Original Format: Shapefiles
* Extra Steps Taken: Clipped to only show rail stations located in Plainfield, NJ
* Challenges: N/A

## Data Quality Issues:
* Some residential parcels had extremely high sale prices, which could be accurate, but there was no way to check.
* The Flood Hazard Layer contained some "low-confidence" or "no estimate" data, but there did not seem to be any located in Plainfield specifically.
* There were not many other obvious missing data-related issues, but most of the datasets that were used just had a lot of data, which was a bit daunting at times. It also made it more challenging to identify any possible gaps in the data.
