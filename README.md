# Electric Vehicle Adoption vs Clean Electricity

An interactive data visualization exploring the relationship between 
**EV adoption** (new electric cars sold annually) and the **cleanliness 
of national electricity systems** (share of electricity from low-carbon 
sources), built as a Data Visualization course project at SRH Berlin.

**Hypothesis:** Countries with cleaner electricity grids tend to adopt 
electric vehicles more rapidly.

---

## Live Visualization

Open `index.html` in a browser, or serve locally to avoid CORS issues:
```bash
python -m http.server 8000
# then open http://localhost:8000
```

---

## Features

**Map (Leaflet + Marker Clusters)**
- Bubble size = EV sales volume
- Bubble color = Clean electricity share (%)
- Click clusters to expand into individual countries
- Click markers for country-year details

**Scatter Plot (D3.js)**
- X-axis: Clean electricity share (%)
- Y-axis: EV sales
- Hover for country details
- Brush to highlight corresponding map markers
- Zoom and pan support

**Filters**
- Year selector — view a specific year or all years combined
- Region selector — filter by world region

---

## Project Structure
---

## Data Pipeline

1. `main.py` merges `ev_sales.csv` + `energy_emissions.csv` → `merged_data.csv`
2. `task7_8.html` joins merged data with country GeoJSON → `master_data.geojson`
3. `index.html` loads `master_data.geojson` and renders map + scatter plot

---

## Technologies

| Layer | Technology |
|-------|-----------|
| Map | Leaflet.js + MarkerCluster |
| Chart | D3.js |
| Preprocessing | Python (pandas) |
| Data format | CSV, GeoJSON |

---

## Data Sources

- **EV Sales:** IEA Global EV Outlook 2025, processed by Our World in Data —
  [CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/)
- **Clean Electricity:** World Energy Data 1990–2020 via Kaggle —
  World Bank Terms of Use

---
