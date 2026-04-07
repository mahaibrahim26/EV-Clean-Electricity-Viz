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
