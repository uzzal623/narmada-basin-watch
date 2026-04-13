# Narmada Basin Watch
## Automated Vegetation & Water Body Monitoring using Sentinel-2

A Python-based geospatial analysis pipeline for monitoring vegetation health and water body dynamics in the **Narmada River Basin, India** — one of India's most ecologically and hydrologically significant river systems, spanning ~98,796 km² across Madhya Pradesh, Maharashtra, and Gujarat.

---

## Project Overview

This notebook demonstrates an end-to-end automated workflow for satellite image processing and spatial data analytics using **Google Earth Engine (GEE)** and Python. It directly addresses key tasks relevant to integrated river basin management:

- **Spectral index computation** — NDVI, NDWI, NDBI from Sentinel-2 multispectral imagery
- **Time-series analysis** — Monthly vegetation and water body trends across the basin
- **Interactive Web mapping** — Geemap + Folium-based map with layer toggle
- **Statistical reporting** — Basin-level and sub-region aggregated statistics
- **Automated cloud-masked image processing** — Production-quality preprocessing pipeline

---
## Tools & Libraries

| Tool | Purpose |
|---|---|
| Google Earth Engine (GEE) | Cloud-based satellite data access & processing |
| `earthengine-api` | GEE Python client library |
| `geemap` | Interactive GEE map visualization |
| `folium` | Leaflet-based interactive maps |
| `geopandas` | Vector data manipulation |
| `rasterio` | Raster data I/O |
| `plotly` | Interactive time-series charts |
| `pandas` / `numpy` | Data manipulation |
| `matplotlib` | Static visualization |

---

##  Key Outputs

1. **Monthly NDVI Time Series** — Seasonal vegetation health patterns across the Narmada basin
2. **NDWI Water Body Map** — Surface water extent mapping
3. **Interactive Multi-layer Map** — Toggle NDVI / NDWI / True Colour / Basin Boundary
4. **Vegetation Class Distribution** — Pixel-level NDVI class breakdown (dense forest, sparse vegetation, bare soil, water)
5. **Basin Statistics Table** — Mean, min, max, std dev per spectral index

---

##  Getting Started (Google Colab)

### Step 1 — Get a free GEE account
Sign up on google earth engine with your google account and create a cloud project

### Step 2 — Open the notebook in Colab
Click the "Open in Colab" badge above, or upload `narmada_basin_monitor.ipynb` 

### Step 3 — Run cells in order
```
Cell 1: Install dependencies     
Cell 2: Authenticate GEE   
Cell 3–4: Define study area     
Cell 5–7: Load & process imagery 
Cell 8–9: Visualizations         
Cell 10: Statistics           
```

---

## Study Area

The **Narmada River Basin** drains an area of ~98,796 km² and originates at Amarkantak (Madhya Pradesh). This analysis focuses on the full basin extent approximately bounded by:

```
Longitude: 72.5°E – 81.8°E
Latitude:  21.2°N – 23.8°N
```

---

## Repository Structure

```
narmada-basin-watch/
├── narmada_basin_monitor.ipynb   # Main analysis notebook (run in Colab)
├── README.md                     # This file
├── LICENSE                       # License
└── outputs/                      # (auto-created) Exported maps & charts
```

---

## Why the Narmada Basin?

The Narmada is one of India's most hydrologically and ecologically significant rivers, spanning ~98,796 km² across four states. I chose it as the study area because:

- It represents a complex, multi-stakeholder river basin with active land-use pressures
- Long-term vegetation and water body monitoring is directly relevant to integrated basin management
- Rich publicly available satellite data (Sentinel-2, Landsat) makes it ideal for demonstrating automated geospatial workflows

The pipeline developed here demonstrates skills applicable to real-world river basin decision-support systems — monitoring land cover change upstream of major reservoirs, tracking riparian zone health, and detecting seasonal water body dynamics.

---

## Author

**Uzzal Saha**  
M.Tech Graduate, Computer Science & Engineering, IIT Indore  
[github.com/uzzal623](https://github.com/uzzal623)

## License
This project is licensed under the MIT License.