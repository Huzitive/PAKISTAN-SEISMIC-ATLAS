# 🇵🇰 Pakistan Seismic Atlas
### An Interactive Geospatial Visualization of Earthquake Distribution and Tectonic Activity

<p align="center">
  <strong>Geophysics · Seismology · GIS · Remote Sensing · Earth Observation</strong>
</p>

---

## 🌍 Overview

**Pakistan Seismic Atlas** is an interactive geospatial visualization project designed to explore earthquake distribution, focal depths, magnitude patterns, and tectonic activity across Pakistan and its surrounding regions.

The project combines earthquake catalog data, active fault traces, tectonic plate boundaries, and geospatial administrative boundaries into a unified interactive mapping environment.

Built using JavaScript and Leaflet.js, the atlas provides an accessible way to investigate regional seismicity and understand the spatial relationship between earthquake activity and tectonic structures.

## ✨ Key Features

### 1. Interactive Earthquake Mapping
- Geographic visualization of earthquake epicentres.
- Magnitude-dependent marker sizing.
- Focal-depth-based color classification.
- Highlighting of significant earthquakes (M ≥ 6.5).
- Interactive markers with detailed earthquake information.
- Direct links to individual USGS earthquake records.

### 2. Tectonic and Geological Visualization

Explore multiple geospatial datasets through independently toggleable map layers:

- **Earthquake Distribution:** Spatial distribution of recorded seismic events.
- **GEM Active Faults:** Mapped and inferred active fault traces.
- **Plate Boundaries:** Regional tectonic plate boundaries.
- **Earthquake Concentration:** Heatmap representation of seismic event concentration.
- **Pakistan Regions:** Administrative boundaries and regional labels.

### 3. Seismic Data Analysis

The dashboard automatically calculates and displays:

- Total earthquakes matching the selected filters.
- Number of earthquakes with reported moment magnitude Mw ≥ 6.0.
- Mean reported magnitude.
- Focal depth distribution.
- Three most concentrated fixed 2° geographic grid cells.

### 4. Interactive Filtering

Explore the earthquake catalog using:

- Minimum magnitude threshold.
- Custom start date.
- Custom end date.
- Reset filters and map view.

### 5. Statistical Visualizations

The atlas includes three analytical charts:

- Annual earthquake frequency (2000–2026).
- Magnitude distribution.
- Focal depth distribution.

All statistical visualizations update dynamically when the filters change.

---

## 🗺️ Geographic Coverage

The atlas covers Pakistan and surrounding tectonically active regions.

| Parameter | Coverage |
|---|---|
| Western longitude | 59° E |
| Eastern longitude | 78° E |
| Southern latitude | 22° N |
| Northern latitude | 38° N |
| Catalog start | 1 January 2000 |
| Catalog end | 28 October 2026 |
| Minimum magnitude | M 4.0 |

The regional extent includes seismic activity associated with the broader Himalayan, Hindu Kush, Balochistan, and surrounding tectonic systems.

## 🛠️ Technology Stack

| Technology | Application |
|---|---|
| HTML5 | Application structure |
| CSS3 | Dashboard styling and responsive layout |
| JavaScript | Data processing and interactivity |
| Leaflet.js | Interactive geospatial mapping |
| Leaflet.heat | Earthquake concentration visualization |
| SVG | Statistical charts |
| NASA EOSDIS GIBS | Terrain and shaded-relief basemap |

## 📡 Data Sources

This project incorporates publicly available geospatial and scientific datasets.

| Dataset | Source | Purpose |
|---|---|---|
| Earthquake Catalog | USGS Earthquake Hazards Program | Earthquake locations, magnitude, depth and time |
| Active Faults | GEM Foundation Global Active Faults 2019 | Active fault visualization |
| Plate Boundaries | Bird PB2002 | Regional tectonic boundaries |
| Administrative Boundaries | OCHA/WFP Pakistan COD-AB | Pakistan regional boundaries |
| Terrain | NASA/METI ASTER GDEM via NASA EOSDIS GIBS | Shaded-relief basemap |

## 📊 Seismic Classification

### Focal Depth

Earthquakes are classified into three focal-depth categories:

| Classification | Depth | Map Color |
|---|---|---|
| Shallow | 0–less than 70 km | Cyan |
| Intermediate | 70–less than 300 km | Amber |
| Deep | 300–700 km | Magenta |

### Magnitude Representation

Earthquake marker sizes increase with magnitude.

- Smaller markers represent lower-magnitude events.
- Larger markers represent stronger earthquakes.
- Events with magnitude ≥ 6.5 receive an additional visual glow.

## 🚀 Getting Started

The project is a standalone HTML application.

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/pakistan-seismic-atlas.git
```

### 2. Open the project

Navigate to the project directory:

```bash
cd pakistan-seismic-atlas
```

### 3. Run the application

Open `index.html` in your web browser.

Alternatively, run a local development server:

```bash
python -m http.server 8000
```

Visit:

```text
http://localhost:8000
```

**Note:** An active internet connection is required to load the external Leaflet libraries and NASA GIBS map tiles. The earthquake and vector datasets are embedded in the HTML file.

## ⚠️ Scientific Considerations and Limitations

This atlas is intended for geospatial exploration and educational/research visualization.

Several considerations are important when interpreting its results:

- Earthquake catalog completeness varies across time and geographical regions.
- Different magnitude scales are present in the catalog.
- Earthquake events include aftershocks.
- Mean magnitude calculations combine reported magnitude types.
- The Mw ≥ 6.0 statistic only includes records with reported Mw magnitude types.
- Heatmap intensity is a screen-space kernel estimate and changes with map zoom.
- Fixed 2° grid-cell counts are not normalized by area or time.
- Mapped and inferred fault traces have positional uncertainty.

**Important:** Earthquake concentration should not be interpreted as a direct measurement of seismic hazard or earthquake probability. This project is not an operational earthquake early-warning or prediction system.

## 📜 License and Attribution

The atlas derivative is released under the **Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)** license.

Individual datasets retain their respective licensing conditions:

- USGS Earthquake Hazards Program — Public Domain.
- GEM Global Active Faults 2019 — CC BY-SA 4.0.
- Bird PB2002 — ODC-By 1.0.
- OCHA/WFP Pakistan COD-AB — CC BY-IGO.
- NASA/METI ASTER GDEM — NASA EOSDIS GIBS.

Please retain appropriate source attribution when redistributing or adapting the project.

---

## 🔬 Project Motivation

Pakistan is situated within a complex tectonic environment influenced by the interaction of the Indian, Eurasian, and Arabian plates.

Its geographical position exposes different regions to significant seismic activity, making earthquake distribution and tectonic structures important subjects of geophysical investigation.

This project aims to bring together publicly available seismic and geological information into an interactive visual platform, making regional seismic patterns easier to explore, interpret, and communicate.

**The broader objective is to demonstrate how geospatial technologies can support geophysical research, Earth observation, and scientific data visualization.**

---

<p align="center">
  <strong>Pakistan Seismic Atlas</strong><br>
  Exploring the Earth's tectonic activity through geospatial science.
</p>
