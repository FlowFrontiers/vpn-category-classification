# Cross-Domain Application Category Classification of WireGuard VPN Traffic

Code accompanying the paper *"Cross-Domain Application Category Classification of
WireGuard VPN Traffic Using Early-Flow Fingerprints"* (CNSM 2026).

This repository contains the full preprocessing, training, evaluation, and
plotting pipeline used in the paper.

## Notebooks

- `00_preprocessing.ipynb` — builds the FlowFeatures and SPLT representations from the dataset
- `01_CrossDomain_CNN1D_SPLT.ipynb` — multi-scale CNN1D on SPLT (cross-domain transfer)
- `02_CrossDomain_RF_XGB_SPLT.ipynb` — Random Forest / XGBoost on flattened SPLT (cross-domain transfer)
- `03_CrossDomain_RF_XGB_FlowFeatures.ipynb` — Random Forest / XGBoost on FlowFeatures (cross-domain transfer)
- `04_Graphical_Results.ipynb` — figures and tables reported in the paper

## Dataset

The matched-capture WireGuard dataset is described in the accompanying *Data in
Brief* data article and archived on Zenodo:

- Data article: Y. S. Razooqi and A. Pekar, "A flow-level dataset of WireGuard
  tunnel traffic with matched encrypted-side features and application labels,"
  *Data in Brief*, vol. 66, p. 112696, 2026.
  doi:[10.1016/j.dib.2026.112696](https://doi.org/10.1016/j.dib.2026.112696)
- Dataset archive (Zenodo): [10.5281/zenodo.18945858](https://doi.org/10.5281/zenodo.18945858)

Obtain the dataset from the links above and place it under `dataset/` to run the
notebooks.

## Authors

Yasameen Sajid Razooqi and Adrian Pekar — FlowFrontiers Research Group,
Department of Networked Systems and Services, Budapest University of Technology
and Economics.
