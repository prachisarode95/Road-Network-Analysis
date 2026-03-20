# Road Network Analysis — Hyderabad, India

Extracts, analyzes and visualizes the drivable road network of Pune 
from OpenStreetMap. Demonstrates road attribute analysis and spatial 
data pipeline skills relevant to HD mapping workflows.

## Output Preview
[paste your map image here after uploading it to the repo]

## What This Project Does
- Downloads live road network data from OpenStreetMap using OSMnx
- Analyzes road type distribution, speed limit coverage, and lane data
- Produces a road network summary by road classification
- Exports results to GeoPackage format for use in QGIS or downstream pipelines

## Key Results
- Total road network length: [your number] km
- Total intersections: [your number]
- Total road segments: [your number]
- Speed limit data coverage: [your number]%

## Data Quality Observations
- [X]% of road segments are missing speed limit attributes
- [X]% are missing lane count data
- This reflects known OSM data completeness challenges in Indian cities

## Tech Stack
Python · OSMnx · GeoPandas · NetworkX · Matplotlib · GeoPackage

## How to Run
1. Open `notebooks/01_road_network_analysis.ipynb` in Google Colab
2. Run all cells top to bottom
3. Outputs saved to `outputs/` folder
