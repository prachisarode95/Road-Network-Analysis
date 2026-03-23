# Road Network Analysis — Hyderabad, India

Geospatial analysis of Hyderabad's road network using OpenStreetMap data.

---

## Interactive Map
> Open `outputs/hyderabad_interactive_map.html` in any browser

![Road Network]()

---

## Project Workflow

1. Download live road network data from OpenStreetMap
2. Extract and analyze HD-map-relevant road attributes
3. Compute graph statistics and identify critical junctions
4. Implement Dijkstra and A* shortest path routing
5. Generate isochrone maps showing drivable coverage zones
6. Process GPS trajectory data with stop detection
7. Export all results to GeoPackage format
8. Produce a fully interactive browser-based map

---

## Key Results

| Metric | Value |
|--------|-------|
| Total intersections | 137,483 |
| Total road segments | 357,569 |
| Total road length | 10,950 km |
| Average circuity | 1.033 |
| 15-min isochrone area | ~257 km² |
| Shortest path (Charminar to Airport) | ~28 km |

---

## Data Quality Observations

OSM attribute coverage for Hyderabad reflects typical completeness
patterns for Indian cities. Geometry and road classification are
well-represented. Operational attributes (speed limits: 3.0%,
lane count: 1.4%) show low coverage — a known challenge in OSM
for this region. Infrastructure flags (bridges: 0.2%, tunnels:
0.09%) align with expected physical counts for the city.

---

## Output Maps

| Map | Description |
|-----|-------------|
| `hyderabad_road_network.png` | Full network colored by road type |
| `hyderabad_routing.png` | Dijkstra vs A* comparison |
| `hyderabad_gradient_map.png` | Road gradient / elevation |
| `hyderabad_centrality.png` | Intersection betweenness centrality |
| `hyderabad_isochrone.png` | 5/10/15 min drive zones |
| `trajectory_stops.png` | GPS stop detection |

---

## Tech Stack

| Tool | Purpose |
|------|---------|
| OSMnx | Road network download & querying |
| GeoPandas | Spatial data processing |
| NetworkX | Graph analysis & routing |
| MovingPandas | Trajectory & stop detection |
| Folium | Interactive HTML map |
| Matplotlib | Static visualizations |

---

## How to Run

1. Open `notebooks/01_road_network_analysis.ipynb` in Google Colab and run.
2. Download `outputs/hyderabad_interactive_map.html`
4. Open in browser to explore the interactive map

---

## Repository Structure
```
road-network-analysis/
├── notebooks/
│   └── 01_road_network_analysis.ipynb
├── outputs/
│   ├── hyderabad_road_network.gpkg
│   ├── hyderabad_interactive_map.html
│   ├── hyderabad_road_summary.csv
│   └── *.png  (6 static maps)
├── requirements.txt
└── README.md
```
