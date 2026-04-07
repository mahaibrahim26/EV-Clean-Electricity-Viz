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
