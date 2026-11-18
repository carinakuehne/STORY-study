[← STORY-study](../README.md)

<p align="center">
  <img src="../assets/story-logo.png" alt="STORY" width="160">
</p>

<img src="../assets/workstream-3.png" alt="" width="80" align="right">

# RMT Pipelines

<p>
  <a href="https://github.com/RADAR-base"><img src="https://img.shields.io/badge/RMT%20platform-RADAR--base-D85868" alt="RMT platform: RADAR-base"></a>
  <img src="https://img.shields.io/badge/wearable-%C5%8Cura%20ring-6D52A0" alt="Wearable: Ōura ring">
  <img src="https://img.shields.io/badge/python-3.12%2B-E07858?logo=python&logoColor=white" alt="Python 3.12+">
  <img src="https://img.shields.io/badge/data%20collection-ongoing-F0B028" alt="Data collection: ongoing">
</p>

Code for processing and analysing STORY remote measurement technology data (ongoing). Smartphone data were collected with the open-source [RADAR-base](https://github.com/RADAR-base) platform; wearable data come from Ōura smart rings.

## Notebooks

### `STORY_prelim_analysis.ipynb`
Preprocessing and preliminary machine learning analysis predicting ED-15 eating disorder behaviours from fortnightly Ōura windows. As data collection is ongoing, it uses data up to a fixed cut-off date (`DATA_CUTOFF` in the config cell).

### Further folders (tbc)
- `rmt-active/`: active RMT processing and analysis (e.g., ecological momentary assessments)
- `rmt-passive-phone/`: passive RMT processing and analysis (phone sensor data)
- `rmt-passive-oura/`: passive RMT processing and analysis (wearable data)

## Requirements

- Python 3.12+
- `pandas`, `numpy`, `scipy`, `scikit-learn`, `matplotlib`

```bash
pip install pandas numpy scipy scikit-learn matplotlib
```

## Data

Input data is not included in this repository. See main [README](../README.md) for data access.

Rebuilding the ED-15 file from raw data (Appendix B) also needs `free_text_tokens.json` in `DATA_DIR` (not included).
