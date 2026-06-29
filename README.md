# TESS Light Curve Preprocessing

## Project Overview

This project preprocesses TESS (Transiting Exoplanet Survey Satellite) light curve data for AI-based exoplanet detection.

## Preprocessing Steps

1. Read TESS FITS files.
2. Extract TIME, PDCSAP_FLUX, and QUALITY columns.
3. Remove missing (NaN) values.
4. Remove observations with bad QUALITY flags.
5. Normalize the flux values.
6. Apply Sigma Clipping to remove outliers.
7. Detrend the light curves using the Wotan library.
8. Save cleaned light curves as CSV files.
9. Generate before and after preprocessing plots.

## Libraries Used

* NumPy
* Pandas
* Matplotlib
* Astropy
* Lightkurve
* Wotan

## Output Files

* Clean CSV files containing preprocessed light curves.
* Before and after preprocessing plots.

## How to Run

1. Install the required libraries:

pip install -r requirements.txt

2. Open and run the notebook:

TESS Processing.ipynb

## Project Workflow

Raw TESS FITS File
↓
Extract TIME, FLUX, QUALITY
↓
Remove NaN Values
↓
Filter QUALITY Flags
↓
Normalize Flux
↓
Sigma Clipping
↓
Detrending using Wotan
↓
Save Clean CSV Files
↓
Generate Plots
