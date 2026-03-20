# Road Network Analysis — Hyderabad, India

Extracts, analyzes, and visualizes the drivable road network of Hyderabad from OpenStreetMap. Demonstrates road attribute analysis and spatial data pipeline skills relevant to HD mapping workflows.

## Project Workflow
- Downloads live road network data from OpenStreetMap using OSMnx
- Analyzes road type distribution, speed limit coverage, and lane data
- Produces a road network summary by road classification

## Key Results
- Total road network length: 20456.2 km
- Total intersections: 137,483
- Total road segments: 357,569
- Roads with speed limit (data coverage): 3%
- Roads without speed limit (data coverage): 97%

## Data Quality Observations
- 97% of road segments are missing speed limit attributes
- 98.6% are missing lane count data
- This reflects known OSM data completeness challenges in Indian cities.

## Tech Stack
- Python
- OSMnx
- GeoPandas
- NetworkX
- Matplotlib

## Output Preview
[paste map image here]
