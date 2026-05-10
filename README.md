# Bruker XRF PPM Biplot Notebook

An interactive Jupyter notebook for visualizing geochemical data produced by [Bruker Elemental XRF instruments](https://www.bruker.com/en/products-and-solutions/handheld-instruments/xrf-analyzers.html).

[![License: CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-sa/4.0/)

## Note
Not affiliated with Bruker

## Features
- Imports Bruker XRF results CSV files
- Automatically parses data from the most recent calibration block
- Converts Methods calibration weight % to parts per million (PPM) and LOD=0
- Display the results as a formatted table
- Provides an interactive biplot with selectable X and Y axes
- Export cleaned data to CSV

## Usage
Click the Binder button below to launch the notebook in your browser - no installation required.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/arf-berkeley/bruker-xrf-ppm-plot/main?urlpath=%2Fdoc%2Ftree%2Fplot-ppm.ipynb)

## Data Format
The notebook expects a Bruker XRF Results.csv file with the following characteristics:
- First column is `File #`
- Contains a `DateTime` column formatted as `MM-DD-YYYY HH:MM`
- Element columns in weight percent 
- Below detection limit values marked as `< LOD`
- Header rows repeated at the start of each calibration Method block

For more information about Bruker XRF instruments see the
[Bruker XRF Analyzer page](https://www.bruker.com/en/products-and-solutions/handheld-instruments/xrf-analyzers.html).

## Requirements
- pandas
- numpy
- plotly
- ipywidgets
- nbformat

## Notes
- Study CSV file must be in Bruker XRF output format
- Sources CSV file is optional and used for comparison overlays
- Below detection limit values (`< LOD`) are replaced with zero