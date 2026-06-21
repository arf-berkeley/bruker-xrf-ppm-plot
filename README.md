<table>
<tr>
<td>

[![Voila](https://img.shields.io/badge/launch-Voila-blue.svg)](https://mybinder.org/v2/gh/arf-berkeley/bruker-xrf-ppm-plot/main?urlpath=voila%2Frender%2Fplot-ppm-voila.ipynb)

</td>
<td>

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/arf-berkeley/bruker-xrf-ppm-plot/main?urlpath=%2Fdoc%2Ftree%2Fplot-ppm.ipynb)

</td>
<td>

[![License: CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/88x31.png)](https://creativecommons.org/licenses/by-sa/4.0/)

</td>
</tr>
</table>

# XRF PPM Biplot and Ternary Plots for Bruker Tracer Application Mode

Use either an interactive App or a live Jupyter notebook to view geochemical data produced by [Bruker Elemental XRF instruments](https://www.bruker.com/en/products-and-solutions/elemental-analyzers/handheld-xrf-spectrometers.html)*.

\* Not affiliated with Bruker Elemental

## Features
- Imports Bruker XRF Results.csv files
- Parses data using filter widgets
- Converts weight % to parts per million (PPM) and LOD=0
- Display the results as a formatted table
- Provides an interactive biplot and ternary plot with selectable X and Y axes
- Export cleaned and filtered data to CSV

## Usage
Click either the Voila or Binder buttons to launch in your browser then wait about 30 seconds for launch to complete -- no installation required.

**Interactive App Only:**
[![Voila](https://img.shields.io/badge/launch-Voila-blue.svg)](https://mybinder.org/v2/gh/arf-berkeley/bruker-xrf-ppm-plot/main?urlpath=voila%2Frender%2Fplot-ppm-voila.ipynb)

**Editable Jupyter Notebook:**
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/arf-berkeley/bruker-xrf-ppm-plot/main?urlpath=%2Fdoc%2Ftree%2Fplot-ppm.ipynb)

**Offline Use:**
The notebook can run offline provided that a Python kernel such as 
[Miniconda](https://docs.conda.io/en/latest/miniconda.html) is available locally, 
along with the required packages listed below.

## Data Format
The notebook expects a Bruker XRF Results.csv file close to the original. Perhaps edit by substituting Application for other Grouping variables if it's redundant with the Method field.

For more information about Bruker XRF instruments see the
[Bruker XRF Analyzer page](https://www.bruker.com/en/products-and-solutions/elemental-analyzers/handheld-xrf-spectrometers.html).

## Requirements
- pandas
- numpy
- plotly
- ipywidgets
- nbformat

## Credits
Created by N. Tripcevich with assistance from Claude 4.6 Sonnet
