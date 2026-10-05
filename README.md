# WRPC-HSE-Spatial-Assessment-Project
A QGIS-based spatial risk assessment mapping HSE hazard zones and environmental containment strategies for a 40-hectare industrial facility.
# WRPC Predeployment HSE & Spatial Containment Assessment

**Industrial Site Safety, Proximity Analysis, and Environmental Risk Mitigation**

## 📌 Project Overview

This project delivers a high precision, site specific Health, Safety, and Environment (HSE) predeployment spatial risk assessment for the **Warri Refining and Petrochemical Company (WRPC)** in Delta State, Nigeria.

The primary objective is to map operational hazard zones and design physical environmental defenses for **Diamond Energytech Company Limited (DECL)** prior to contractor deployment. By utilizing advanced GIS techniques within a strict 40 hectare operational footprint, this assessment identifies overlapping hazard zones and engineers spatial solutions to protect both personnel and the local ecological system.

## ⚠ Why This Project is Important

Industrial maintenance in highly congested facility zones carries extreme risk. This project addresses the **"cascade effect":** where the failure of one critical asset can trigger adjacent failures due to overlapping blast or thermal radii.

Furthermore, the facility's proximity to the **Ekpan River** creates a high risk topographical pathway. Without strategic predeployment planning, an accidental hydrocarbon spill could easily breach the facility's road boundaries and contaminate the river. This map resolves both the logistical bottleneck of worker safety and the environmental vulnerability of the local waterways.

## 📊 Data Sourcing & Generation

Unlike regional macro assessments that rely on secondary municipal datasets, this micro scale operational model required high precision primary data creation:

* **Basemap Imagery:** High resolution satellite imagery served as the foundational spatial reference for the 40 hectare footprint.
* **Vector Data (Primary Creation):** All infrastructure points (10 tank cluster), 50m thermal and blast buffers, and strategic containment polygons were manually digitized and geometrically verified using precision QGIS tools.

## 🗺️ Map Legend & Visual Symbology

The spatial containment strategy was digitized using precision vertex editing. The map features the following critical layers:

* **Pink Points (DECL Infrastructure):** These represent the exact coordinates of the 10 critical storage tanks and processing assets managed by Diamond Energytech Company Limited.

* **Faint Red Zones (50m Hazard Buffers):** Mathematical 50 meter thermal radiation and blast radii generated around the DECL infrastructure. Their heavy overlap visually proves the extreme asset congestion and cascade risk on site.

* **Bright Green Zone (Cold Zone Safety Area):** A designated offsite safe zone. Because the 50m hazard buffers consume the entire operational cluster, this staging area ensures workers and laydown equipment remain completely outside the danger zone during pre work briefings and rest periods.

* **Yellow Zone (Secondary Containment Bund):** A continuous perimeter polygon designed to ring fence the entire congested 10 tank cluster. Individual tank berms were spatially impossible, so this bund captures catastrophic ground level spills from any asset within the cluster.

* **Red Zone (Runoff Barrier):** Positioned along the topographical gradient, this physical drainage defense ends just right before the roadway. It acts as the final interceptor trench to stop contaminated surface flow from crossing the road and discharging into the Ekpan River.

## 🌐 Technical Methodology & CRS

To ensure absolute metric precision for the blast radii and engineering offsets, the project was locked into a metric coordinate reference system rather than degrees:

* **Coordinate Reference System (CRS):** `EPSG:32632` (WGS 84 / UTM Zone 32N).

* **Tools Utilized:** QGIS Geoprocessing (Buffer Tool), Advanced Digitizing Toolbar (Vertex Tool snapping), and Categorized Symbology (utilizing varying opacities to preserve underlying satellite context).

## 🌍 The Environmental Receptor (Ekpan River)

A core component of this HSE strategy is the **Source Pathway Receptor** model:

* **Source:** The DECL Infrastructure (Pink Points).

* **Pathway:** The internal site gradient leading to the public roadway.

* **Receptor:** The Ekpan River.

By mapping the Red Runoff Barrier just before the road, we establish a mandatory field requirement for interceptor trenches or spill booms. The map visually communicates to site managers exactly where the physical defense line must be drawn to prevent an ecological disaster before hot work even begins.

## ⚠ Project Limitations & Constraints

1. **Topography Dependency:** The efficiency of the Runoff Barrier relies on micro topographical accuracy. Sudden, unmapped local depressions could bypass primary trenches.

2. **Zero Internal Safe Space:** The high density of the facility prevents any internal worker rest areas, introducing logistical friction as teams must transition to the Cold Zone daily.

3. **Macro Bunding:** Individual asset containment was impossible due to congestion, meaning a failure in one tank still floods the immediate base of neighboring tanks within the Yellow Bund.
