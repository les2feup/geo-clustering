# Geospatial Clustering Analysis of Urban Data

![LES2 Banner](https://github.com/les2feup/guidelines/raw/main/src/figures/les2banner.png)

[![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-orange.svg?logo=jupyter)](https://jupyter.org/)
[![Python 3.12](https://img.shields.io/badge/Python-3.12-blue.svg?logo=python&logoColor=white)](https://www.python.org/downloads/release/python-3120/)
[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-yellow.svg)](https://opensource.org/licenses/Apache-2.0)

This repository contains Jupyter Notebooks that demonstrate geospatial clustering techniques applied to urban datasets. The notebooks utilize popular Python libraries such as `pandas`, `geopandas`, `scikit-learn`, and `matplotlib` to perform clustering analysis and visualize the results.

<!--
**Publication**

This work is part of the research published in the following paper: -->

## Notebooks

- [`01_Educational_Hubs.ipynb`](01_Educational_Hubs.ipynb): A basic application that uses K-Means and DBSCAN clustering to characterize the spatial distribution of educational institutions in Porto, Portugal.

- [`02_Wildfire_Hotspots_in_Portugal.ipynb`](02_Wildfire_Hotspots_in_Portugal.ipynb): An advanced application that employs HDBSCAN clustering to identify and analyze wildfire hotspots across Portugal.

- [`03_Spatiotemporal_Vulnerability.ipynb`](03_Spatiotemporal_Vulnerability.ipynb): A end-to-end application based on [VERUS](https://github.com/les2feup/verus), which combines OPTICS and K-Means clustering to assess spatiotemporal vulnerability in urban areas based on various points of temporal influence.

## Quick Start

### Running without installation

You can run the notebooks directly in Google Colab without any local installation. Simply click the "Open in Colab" badge at the top of each notebook.

<a href="https://colab.research.google.com/github/les2feup/geo-clustering/blob/main/01_Educational_Hubs.ipynb" target="_blank">
<img src="https://img.shields.io/badge/Open%20in-Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white" alt="Open In Colab"/>
</a>

> ⚠️ **Note:** Colab provides a temporary environment. Your work will be lost after your session ends, so remember to download any important data or notebooks.

## Running Locally in VSCode

To run the notebooks locally, follow these steps:

1. Clone the repository:

    ```bash
    git clone https://github.com/les2feup/geo-clustering.git
    cd geo-clustering
    ```

2. Create a virtual environment and activate it:

    ```bash
    python3 -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

4. Open the repository in VSCode and launch Jupyter Notebooks.

## Dependencies

Python 3.12 is the tested version for running the notebooks locally. The complete
dependency specification is maintained in [`requirements.txt`](requirements.txt).

- **Notebook runtime:** `ipykernel`, `requests`
- **Geospatial analysis:** `geopandas`, `osmnx`, `verus`
- **Clustering and machine learning:** `scikit-learn`, `hdbscan`
- **Visualization:** `matplotlib`, `contextily`

## License

This project is licensed under the Apache 2.0 License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- This project was developed at the Laboratory of Emerging Smart Systems (LES2) at the Faculty of Engineering of University of Porto (FEUP), Portugal.
- This work was supported by the Associate Laboratory Advanced Production and Intelligent Systems – ARISE LA/P/0112/2020 (DOI 10.54499/LA/P/0112/2020), by the Base Funding (UIDB/00147/2020) and Programmatic Funding (UIDP/00147/2020) of the R&D Unit Center for Systems and Technologies -- SYSTEC, and by the Fundação para a Ciência e a Tecnologia (FCT) through the PhD scholarship (2024.02446.BD).
