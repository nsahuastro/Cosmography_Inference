# Cosmography Inference with DSPLs and Cosmological Probes

This repository contains code and notebooks for cosmological inference using double source plane lenses (DSPLs) and combining constraints from CMB, SNe Ia, and BAO data. The main workflow is implemented in the notebook `cosmology_using_Beta12_wCDM.ipynb`.

## Workflow Overview

- **Data Preparation:** Reads in DSPL lens model outputs, CMB chains, SNe Ia, and BAO chains.
- **Distance Ratio Calculation:** Computes cosmological distance ratios for lensing systems using wCDM and LCDM models.
- **MCMC Sampling:** Performs MCMC sampling to constrain cosmological parameters (w, Ω_m) using observed DSPL ratios.
- **Posterior Analysis:** Analyzes MCMC chains, computes medians, confidence intervals, and visualizes results.
- **Combining Constraints:** Uses kernel density estimation (KDE) to combine posteriors from DSPLs, CMB, SNe, and BAO, both in 1D and 2D.
- **Visualization:** Generates triangle plots and 2D contour plots for combined constraints.

## Usage

- Run the notebook `cosmology_using_Beta12_wCDM.ipynb` in Jupyter or VSCode.
- Ensure all required data files (lens model outputs, CMB chains, SNe and BAO chains) are present in the working directory.
- The notebook is modular and can be adapted for other lens systems or cosmological probes.

## Dependencies

- Python 3.x
- numpy, scipy, pandas, matplotlib, seaborn
- astropy, getdist, emcee, chainconsumer, h5py
- tqdm, joblib

## Citation

If you use this code or results in your work, please cite:

Sahu et al. (2019), [https://ui.adsabs.harvard.edu/abs/2019MNRAS.482.1121S/abstract](https://ui.adsabs.harvard.edu/abs/2019MNRAS.482.1121S/abstract)
