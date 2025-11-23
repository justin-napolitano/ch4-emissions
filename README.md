# CH4 Emissions Analysis

This repository contains a comprehensive Jupyter Book project analyzing global methane (CH4) emissions from rice paddies. It includes data exploration, replication of academic papers, hypothesis testing, and geospatial analysis to better understand methane emission estimates and their discrepancies.

## Features

- Data exploration and visualization of methane emissions data.
- Replication and testing of the University of Malaysia's methane emissions paper.
- Hypothesis testing on emission data distributions.
- Geospatial merging and mapping of methane emission data.
- Automated build pipeline for the Jupyter Book site.

## Tech Stack

- Primary language: Jupyter Notebooks (Python)
- Key libraries: pandas, geopandas, matplotlib, scipy, folium
- Build tools: Jupyter Book, Python subprocess for automation

## Getting Started

### Prerequisites

- Python 3.x
- pip package manager

### Installation

1. Clone the repository:

```bash
git clone https://github.com/justin-napolitano/ch4-emissions.git
cd ch4-emissions
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

### Build and Run

The project uses a Python build script to automate dependency installation and Jupyter Book build:

```bash
python python_build.py
```

Alternatively, you can manually build the Jupyter Book:

```bash
jupyter-book build jupyter-book
```

Open the generated HTML files in the `jupyter-book/_build/html` directory to view the reports.

## Project Structure

```
ch4-emissions/
├── data/                 # Raw and processed data files
├── jupyter-book/         # Jupyter Book source files
│   ├── notebooks/        # Analysis notebooks
│   ├── _config.yml       # Jupyter Book configuration
│   ├── _toc.yml          # Table of contents
│   └── index.md          # Book introduction
├── python_build.py       # Build and deployment automation script
├── website/              # Website related files (assumed)
```

## Future Work / Roadmap

- Add detailed documentation and descriptions for each notebook.
- Automate data updates and integrate with live data sources.
- Enhance visualizations with interactive maps and dashboards.
- Extend analysis to other methane emission sources beyond rice paddies.
- Deploy the Jupyter Book site with continuous integration for live updates.

---

*Note: Some assumptions were made regarding the website directory and data files based on typical project structures.*