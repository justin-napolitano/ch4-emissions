---
slug: github-ch4-emissions
title: CH4 Emissions Analysis with Jupyter Book and Python
repo: justin-napolitano/ch4-emissions
githubUrl: https://github.com/justin-napolitano/ch4-emissions
generatedAt: '2025-11-23T08:41:33.175740Z'
source: github-auto
summary: >-
  This project analyzes methane emissions from rice paddies using Jupyter Book,
  focusing on data sources, statistical testing, and geospatial analysis.
tags:
  - methane
  - ch4-emissions
  - geospatial-analysis
  - jupyter-book
  - climate-data
  - statistical-testing
  - python
  - geospatial
  - pandas
  - folium
seoPrimaryKeyword: methane emissions analysis
seoSecondaryKeywords:
  - Jupyter Book project
  - data visualization
  - statistical methods
  - geospatial analysis
  - FAOSTAT data
  - climate TRACE
  - emission estimates
seoOptimized: true
topicFamily: datascience
topicFamilyConfidence: 0.95
topicFamilyNotes: >-
  The post focuses extensively on data analysis workflows including geospatial
  analysis, statistical testing, Jupyter Book structured notebooks, and data
  science tools like pandas, geopandas, and scipy. The subject matter fits
  squarely within the datascience family, and the explicit slug match
  ('github-ch4-emissions') confirms this. While automation aspects exist, they
  support the data science workflow rather than being the main focus.
kind: project
id: github-ch4-emissions
---

# CH4 Emissions Analysis: Technical Overview

## Motivation

Methane (CH4) is a potent greenhouse gas with significant impact on climate change. Rice paddies contribute approximately 8% of global methane emissions, making accurate estimation vital for environmental policy and mitigation strategies. This project addresses discrepancies in methane emission estimates, particularly those reported by the Food and Agricultural Organization of the United Nations (FAOSTAT) and research from the University of Malaysia.

## Problem Statement

Current global methane emission estimates rely on varying methodologies and data sources. FAOSTAT uses official government data with conversion factors, which may be subject to manipulation or inaccuracy. Alternative estimates, such as those from Climate TRACE, use satellite imaging to estimate cultivated rice paddy areas. The project aims to analyze these differences, replicate academic findings, and test hypotheses about emission distributions.

## Project Composition

The repository is structured as a Jupyter Book project, comprising multiple notebooks that perform different aspects of the analysis:

- **Data Exploration:** Import and visualize methane emission datasets from FAOSTAT and University of Malaysia.
- **Replication of Academic Paper:** Recreate analyses from the University of Malaysia's methane emissions paper, including data merging and difference calculations.
- **Hypothesis Testing:** Statistical tests (e.g., Shapiro-Wilk for normality) to validate claims about emission data distributions.
- **Geospatial Analysis:** Merge emission data with geographic shapefiles to enable mapping and spatial visualization.
- **Blog Posts:** Summaries and discussions of findings in narrative form.

Automation is handled via a Python script (`python_build.py`) that installs dependencies and builds the Jupyter Book site using subprocess calls to `jupyter-book` commands.

## Implementation Details

- **Data Sources:** Excel and CSV files containing methane emission data from 2015 to 2021, including country-level estimates.
- **Libraries:** Utilizes pandas for data manipulation, geopandas for spatial data, matplotlib and folium for visualization, and scipy for statistical testing.
- **Build Pipeline:** The build script automates cleaning and building the Jupyter Book, committing changes, and pushing to a remote repository (details inferred but incomplete).
- **Jupyter Book Configuration:** The `_config.yml` file sets book metadata, execution policies (forcing notebook re-execution), and repository links.
- **Table of Contents:** Defined in `_toc.yml` to organize notebooks into thematic sections such as blog posts, paper replication, and data exploration.

## Practical Considerations

- The data paths in notebooks are absolute and local to the developer's environment; these should be parameterized or documented for portability.
- Statistical testing confirms non-Gaussian distributions, requiring non-parametric methods for hypothesis testing.
- Geospatial merges exclude Antarctica and handle coordinate reference system transformations.
- The build automation script relies on an undefined `utility_functions` module, which should be included or documented.

## Summary

This project provides a reproducible framework for analyzing methane emissions from rice paddies, combining data science, geospatial analysis, and statistical testing. It serves as a reference implementation for validating emission estimates and exploring methodological discrepancies in environmental data reporting. The Jupyter Book format facilitates documentation and dissemination of findings.

Future work should focus on improving data accessibility, expanding analyses, and enhancing automation for deployment and continuous integration.

