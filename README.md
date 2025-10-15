# DURUM: Database of Urban RUnoff Microplastics

**Paper title:** *Standardizing microplastic data in urban runoff: Development and applications of the DURUM database*

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)]()
[![Data: CC BY 4.0](https://img.shields.io/badge/Data-CC%20BY%204.0-blue.svg)]()

This repository hosts the DURUM dataset and companion notebook for the paper:

> Standardizing microplastic data in urban runoff: Development and applications of the DURUM database

## Authors (full list)
- Abdul Mobin Ibna Hafiz
- Ebrahim Ahmadisharaf
- Maryam Salehi
- Tim H. M. van Emmerik
- Jeffrey Farner
- Jason C. White
- Yanxu Zhang
- Tamara Galloway
- Naipeng Han
- Wen Zongguo

## Abstract (from manuscript)
Urban runoff represents a critical transport pathway of microplastics (MPs) connecting terrestrial sources to aquatic ecosystems. However, predictive modeling capabilities for microplastic transport and fate in urban systems, which can assist mitigation measures, remain severely constrained by the absence of comprehensive standardized datasets. This study presents the Database of Urban RUnoff Microplastics (DURUM), the first dedicated global database of MPs in urban stormwater systems, encompassing surface runoff from streets, residential catchments, commercial districts, industrial areas, and urban drainage infrastructure, systematically compiling and harmonizing data from 28 peer-reviewed studies spanning 15 countries and encompassing 180 measurement records collected between 2018-2024. DURUM integrates and standardizes MP concentrations, particle size distributions, morphological characteristics, polymer compositions, and hydrometeorological metadata through systematic harmonization protocols developed in this study to support microplastic transport and fate modeling, calibration, and validation across diverse urban environments. The standardization protocol converts diverse reporting units to particles per liter, harmonizes size classification schemes, and establishes consistent metadata formats to enable future database expansion and inter-study comparisons. MP concentrations exhibited substantial variability spanning nearly five orders of magnitude, ranging from 0.16 to 18,966 particles/L across residential, commercial, industrial, and transportation corridors. Mass concentrations were not consistently reported across studies and thus excluded from standardization; all analyses are based on particle number concentrations. The geometric mean of 33.2 particles/L reflects the log-normal distribution typical of environmental contaminants, though concentrations varied dramatically by land use type and methodological approach. Fibrous particles dominated the morphological inventory across all records (38.9%), followed by fragments (33.5%), while polyethylene (27.4%) and polypropylene (26.5%) represented the most abundant polymer classes. Hydrometeorological parameters including antecedent dry periods, rainfall intensity, and temperature were inconsistently reported (present in only 23% of records), limiting temporal variability analysis and representing a critical data standardization need for future transport modeling applications. Reported particle concentrations varied significantly by analytical method, with studies detecting particles ≤100 μm yielding median concentrations approximately 10-fold higher than those limited to >100 μm detection ranges (median: 70 vs. 7 particles/L), reflecting the expected increase in particle abundance with decreasing size while underscoring that analytical method selection fundamentally constrains cross-study comparability. This database addresses the absence of standardized, globally-compiled datasets necessary for predictive modeling of MP transport in urban stormwater systems. By harmonizing concentration data, particle characteristics, and environmental metadata across diverse geographic and methodological contexts, DURUM provides the empirical foundation for developing and validating mechanistic transport models, statistical relationships, and machine learning frameworks capable of predicting MP fate across varied urban compartments. This standardized dataset enables robust model calibration, cross-validation, and uncertainty quantification, essential for evidence-based pollution control strategies. While this compilation focuses on microplastics (<5 μm), nanoplastics (<1 μm) represent an emerging concern with greater toxicological significance but present substantial analytical challenges that currently preclude systematic database inclusion.
KEYWORDS: Microplastics; Modeling; Sampling; Plastic Pollution; Stormwater; Runoff.

---

## Repository Contents
- `data/` — main dataset file(s) (CC BY 4.0).
- `notebooks/` — Jupyter notebooks to reproduce basic summaries/visualizations.
- `docs/` — documentation assets such as the data dictionary.

> **Note:** If your Excel file is larger than 100 MB, GitHub web upload will fail. In that case, use Git LFS (see bottom of this README).

---

## Quick Start
1. Download this repository (Code → Download ZIP) or clone it.
2. Place your files:
   - `Urban Runoff MP Database_072025.xlsx` into `data/`
   - `Database code.ipynb` into `notebooks/`
3. Open `notebooks/Database code.ipynb` in Jupyter Lab or Google Colab.
4. Ensure the Excel file path in the notebook points to `data/Urban Runoff MP Database_072025.xlsx`.
5. Run all cells to reproduce summary outputs.

---

## Citation
If you use DURUM, please cite: **Ibna Hafiz et al. (2025)** — *Standardizing microplastic data in urban runoff: Development and applications of the DURUM database*. 2025. Version 0.1.0. DOI: *TBD*.

A machine-readable citation is provided in `CITATION.cff`.

---

## Licenses
- **Code** is licensed under **MIT** (see `LICENSE`).
- **Data** is licensed under **CC BY 4.0** (see `LICENSE-DATA`).

---

## Data Dictionary
See **[`docs/DATA_DICTIONARY.md`](docs/DATA_DICTIONARY.md)** for column descriptions and controlled vocabularies.

---

## Contributing
Contributions (issues, pull requests) are welcome. See `CONTRIBUTING.md`.

---

## Git LFS (only if your Excel >100 MB)
If the Excel file is ≥100 MB, GitHub web upload will be blocked. Either split the file or set up Git LFS locally:

```bash
# one-time install
git lfs install
# track large file types
git lfs track "*.xlsx"
git add .gitattributes
git add data/Urban\ Runoff\ MP\ Database_072025.xlsx
git commit -m "Add dataset via LFS"
git push
```
