# 🌋 Spatial Mismatch: Mt. Galunggung Vulnerability Index

**TL;DR:** Engineered a spatial overlay pipeline to intersect continuous volcanic hazard zones (KRB) with rigid administrative boundaries, identifying high-risk population clusters trapped in jurisdictional blind spots.

* **Role:** GIS Researcher / Spatial Data Analyst
* **Tools:** Python (`GeoPandas`, `Shapely`) • GADM Shapefiles • Spatial Intersection • Google My Maps
* **Live Map:** [Insert Link to your Google My Maps or Dashboard Here]

## 🚨 The Problem
Disaster mitigation efforts often suffer from "Spatial Mismatch." Natural hazards like volcanic lava flows and ash trajectories do not respect arbitrary political borders. When emergency management relies solely on administrative sub-district (Kecamatan) data, they lose visibility on the specific populations living directly inside high-risk topographic zones. 

## 🛠️ The Approach
* **Hazard Modeling:** Programmatically generated multi-tiered hazard buffer zones (KRB 1, 2, and 3) radiating from the Mt. Galunggung crater using established historical radius metrics.
* **Geospatial Ingestion:** Loaded and projected official Level-3 administrative shapefiles (GADM) for the Tasikmalaya region into a localized metric coordinate system (UTM 48S).
* **Overlay Intersection:** Executed a complex spatial join (`gpd.overlay`) to slice the rigid political boundaries using the fluid hazard zones, calculating exact exposed hectares and estimating trapped populations based on localized density metrics.

## 📈 The Results
* Built a continuous vulnerability index that isolated specific, hyper-local populations at risk of catastrophic loss, bypassing the standard "whole district" averaging method.
* Extracted multi-layered KML geometric data to generate a highly interactive, enterprise-grade GIS map for stakeholder presentation.
