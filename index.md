---
slug: "github-ch4-emissions"
title: "ch4-emissions"
repo: "justin-napolitano/ch4-emissions"
githubUrl: "https://github.com/justin-napolitano/ch4-emissions"
generatedAt: "2025-11-23T08:20:10.736318Z"
source: "github-auto"
---


# Exploring Global Methane Emissions from Rice Paddies: My Journey with CH4-Emissions

Methane emissions are a critical part of the climate change puzzle, and rice paddies contribute a significant share—about 8% of global human-linked methane emissions. This project, `ch4-emissions`, is my deep dive into understanding these emissions better, questioning existing estimates, and replicating academic work to validate or challenge their findings.

## Motivation

I was inspired by a report from the University of Malaysia that claimed the United Nations underreports methane emissions by roughly 16%. Their methodology seemed questionable to me, so I decided to test their findings by recreating their analyses and comparing them with other data sources like FAOSTAT and Climate TRACE.

Methane is a potent greenhouse gas—over 20 years, it is 80 times more effective at warming the planet than carbon dioxide. Given its impact, accurate measurement is crucial for climate policy and mitigation strategies.

## The Problem

Measuring methane emissions from rice paddies is tricky. Traditional estimates rely on multiplying the hectares of rice cultivation by conversion factors based on government reports, which can be manipulated or inaccurate. On the other hand, newer satellite imaging methods like Climate TRACE offer alternative estimates but may miss small or high-altitude fields.

This discrepancy between datasets motivated me to explore the data, replicate existing studies, and perform statistical tests to understand the differences better.

## How It's Built

The project is structured as a Jupyter Book, combining narrative, code, and visualizations in an accessible format. It includes:

- **Data Exploration:** Using pandas, geopandas, and matplotlib, I explore datasets from FAOSTAT, the University of Malaysia, and Climate TRACE.
- **Replication of Academic Work:** I replicate the University of Malaysia's paper to verify their data processing and conclusions.
- **Hypothesis Testing:** Using statistical tests like Shapiro-Wilk, I check assumptions about data distributions and test differences between years.
- **Geospatial Analysis:** By merging emission data with geographic shapefiles, I create maps to visualize emissions spatially.

Automation is handled via a Python script that installs dependencies and builds the Jupyter Book site using `jupyter-book` commands, making it easy to reproduce and update the analysis.

## Interesting Implementation Details

- The build pipeline automates cleaning and rebuilding the Jupyter Book, committing changes, and pushing updates, which streamlines publishing.
- The notebooks include detailed statistical analysis, including normality tests and non-parametric hypothesis testing, ensuring rigor.
- Geospatial merging uses CRS transformations and GeoJSON outputs to enable mapping and visualization.
- The project carefully compares different methane emission estimates, highlighting the importance of methodology in environmental data.

## Why this project matters for my career

Working on `ch4-emissions` has been a fantastic opportunity to blend data science, environmental science, and software engineering. It sharpened my skills in data analysis, reproducible research, and scientific communication. By tackling a real-world problem with societal impact, I demonstrate my ability to work on interdisciplinary projects that require both technical expertise and domain understanding. This project also showcases my proficiency in automating workflows and building interactive, shareable reports—skills that are highly valuable in data-driven roles.

Overall, this project is a testament to my commitment to rigorous analysis and my passion for addressing climate change through data.

---

Thanks for reading! If you want to explore the code or data, check out the repository [here](https://github.com/justin-napolitano/ch4-emissions).