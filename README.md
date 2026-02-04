# Analyzing the Spatial Alignment Between Public Waste Bins and Pedestrian Mobility in Urban Toronto

## Project Overview
This is a **group project** focused on analyzing the spatial alignment between:
- public waste bin distribution
- pedestrian mobility patterns
- transit accessibility
- population context  
within the City of Toronto.

The objective is to evaluate whether waste bins are spatially aligned with areas of high pedestrian activity and urban demand, using geospatial analysis techniques in Python.

---

## Project Scope
The analysis integrates multiple spatial and contextual layers:
- Waste bin locations
- Pedestrian proxy datasets (sidewalks, activity indicators)
- Public transit access points
- Population and demographic context

All spatial processing, validation, and analysis are performed using **Python (GeoPandas, Shapely, Pandas, NumPy)** in VS Code / Jupyter Notebooks.

---

## Repository Structure

```text
Toronto_Waste_Analytics/
│
├── notebooks/
│   └── Jupyter notebooks used for data loading, validation, and analysis
│
├── waste_bins/
│   └── Waste bin-related spatial references and structure
│
├── pedestrian_proxy/
│   └── Proxy datasets representing pedestrian activity and movement
│
├── transit_points/
│   └── Transit stops and access point structure
│
├── population_context/
│   └── Population and demographic context structure
│
├── .gitignore
└── README.md

> Note: Some folders may appear empty in GitHub. This is intentional and reflects the project structure.
---

## Data Management Policy

### GitHub
This repository contains:
- project structure
- Python code
- Jupyter notebooks
- documentation

### OneDrive (Shared Separately)
Large datasets and raw spatial files (CSV, TXT, GeoJSON, SHP, etc.) are **not stored in GitHub** due to size and versioning constraints.

All team members are expected to:
1. Download the shared datasets from OneDrive
2. Place them into the corresponding local folders
3. Run notebooks and scripts locally

This ensures:
- lightweight repository
- no file size issues
- consistent structure across all team members

---

## Tools & Technologies
- Python 3.x
- GeoPandas
- Pandas
- NumPy
- Shapely
- Jupyter Notebook
- VS Code
- GitHub

---

## Notes
- This repository is intended for collaborative academic work.
- Folder placeholders are used to preserve structure without uploading datasets.
- Any structural changes should be discussed with the group before implementation.
