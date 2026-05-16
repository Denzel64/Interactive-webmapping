# Geospatial Analytics & Web Mapping Projects

This workspace tracks project frameworks, data layering methods, and web exports created using QGIS, OpenLayers, and Leaflet.

---

## 🗺️ Project Framework: Regional Urban Mobility Mapping

### 1. Objective
Design and deploy an interactive web map to track public transport routes, transit hubs, and commuter density corridors without requiring heavy server-side architecture.

### 2. Core Data Layers & Vector Structures
* **Base Layer:** OpenStreetMap standard vector layers for regional road network geometry.
* **Point Data:** Coordinate tracking for primary transit hubs, drop-off stations, and commuter convergence points.
* **Heatmaps:** Population density and peak-hour volume visualization mapped across urban boundaries.

---

## 🛠️ Web Export & Optimization Workflow

When exporting maps via `qgis2web` for public viewing, the deployment follows these criteria to maintain performance:

1. **Layer Control (Leaflet/OpenLayers):** Enabling interactive layer toggles so viewers can switch seamlessly between standard maps, satellite views, and data layers.
2. **Feature Pop-ups:** Configuring lightweight HTML pop-up windows on point vectors to display relevant location metrics (e.g., station name, capacity) when clicked.
3. **File Size Optimization:** Simplifying complex polygon paths and filtering out unnecessary attribute tables before export to ensure rapid page load speeds on mobile and web browsers.
