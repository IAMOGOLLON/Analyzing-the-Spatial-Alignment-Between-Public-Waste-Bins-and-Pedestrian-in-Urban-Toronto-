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
TORONTO_WASTE/
├── data/
│   ├── raw/                   # Original source datasets (never edited). 
│   │   ├── waste_bins/         # Raw waste bin layers (CSV/GeoJSON/Shaefpile)
│   │   ├── transit_points/     # Raw transit stops/routes layers (Txt)
│   │   ├── population_context/ # Raw population tables (CSV)
│   │   └── pedestrian_proxy/   # Raw pedestrian proxy layers (CSV)
│   └── clean/                 # Cleaned/standardized datasets (created by main.py)
├── notebooks/                 # Jupyter notebooks for EDA, QA checks, and analysis (call functions from src/)
├── outputs/                   # Figures, tables, maps, exports for report/dashboard
│
├── src/
│   ├── ui/
│   │   └── overview.py         # Optional: quick-run summary view/sanity checks
│   ├── main.py                 # Orchestrates the full pipeline (load → clean → integrate → save)
│   ├── paths.py                # Centralized project paths (data/raw, data/clean, outputs)
│   ├── __init__.py             # Marks src as a package (enables python -m src.main imports)
│   ├── 01_waste_bins_cleaning_checks.ipynb
│   ├── 02_pedestrian_proxy_cleaning_checks.ipynb
│   ├── 03_transit_points_cleaning_checks.ipynb
│   ├── 04_population_context_checks.ipynb
│   └── 05_analysis_integration.ipynb  # final integration logic
│   └── utils.py                # shared logger and utility helpers
│   └── app_data.py
├── feature_engineering.py  # Spatial grid creation, metrics, and derived features
│   ├── normalization.py
│   ├── feature_engineering.py  # Spatial grid creation, metrics, and derived features
│   ├── integrate.py            # Merge cleaned layers into a common spatial unit (grid/join keys)
│   ├── app_data.py             # Optional: shared data objects/config for UI or notebooks
│   └── utils.py                # Shared utilities (CRS helpers, geometry fixes, logging, QA checks)
│
├── tests/                      # Pytest unit tests (optional but professional)
│   ├── test_data_loader.py         # tests for raw data loading
│   ├── test_data_cleaning.py       # tests for cleaning outputs
│   ├── test_normalization.py       # test normalization
│   └── test_integrate.py           # tests for final integrated dataset
│
├── requirements.txt
├── .gitignore
└── README.md
> Note: Some folders may appear empty in GitHub. This is intentional and reflects the project structure.
```
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
