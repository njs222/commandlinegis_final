# **Command-Line GIS Final Project**
## Housing Parcels Located in Flood Zones (Plainfield, NJ)

Created by: Nicholas Seu

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

[FEMA's National Flood Hazard Layer (NFHL) Viewer ](https://www.arcgis.com/apps/webappviewer/index.html?id=8b0adb51996444d4879338b5529aa9cd)
*Obtained From: ArcGIS.com
*Last Updated:
*Original Format:
*Extra Steps Taken:
*Challenges:
[Union County MODIV Parcel Data](https://njogis-newjersey.opendata.arcgis.com/documents/79789530a56d425082afade9fea64252/about)
* Obtained From: NJGIN
*Last Updated: November 24, 2025 
*Original Format: Shapefile
*Extra Steps Taken: The parcel data was clipped to Plainfield specifically and then filtered to only show parcels that were identified as residential
*Challenges: Initially, it was challenging to figure out how to filter out all of the irrelevant data. I ran into a lot of errors during this process

Who prepared them? How recently were they updated? What format were they originally in? Did you have to do anything to make them mappable (table join, spatial join, geocoding, aggregation, etc.)? Were there any issues with data quality that you had to address?
