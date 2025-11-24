---
slug: github-ch4-emissions-note-technical-overview
id: github-ch4-emissions-note-technical-overview
title: CH4 Emissions Analysis
repo: justin-napolitano/ch4-emissions
githubUrl: https://github.com/justin-napolitano/ch4-emissions
generatedAt: '2025-11-24T18:32:13.965Z'
source: github-auto
summary: >-
  This repo analyzes global methane (CH4) emissions from rice paddies using
  Jupyter Book. It offers data exploration, replication of research, hypothesis
  testing, and geospatial analysis.
tags: []
seoPrimaryKeyword: ''
seoSecondaryKeywords: []
seoOptimized: false
topicFamily: null
topicFamilyConfidence: null
kind: note
entryLayout: note
showInProjects: false
showInNotes: true
showInWriting: false
showInLogs: false
---

This repo analyzes global methane (CH4) emissions from rice paddies using Jupyter Book. It offers data exploration, replication of research, hypothesis testing, and geospatial analysis. 

### Key Features
- Visualize methane emissions data.
- Replicate findings from a University of Malaysia paper.
- Hypothesis testing for emission data distributions.
- Geospatial mapping and merging of data.
- Automated build pipeline for easy site generation.

### Tech Stack
- **Language**: Jupyter Notebooks (Python)
- **Libraries**: pandas, geopandas, matplotlib, scipy, folium
- **Build Tools**: Jupyter Book, Python for automation

### Quick Start
1. Clone the repo:
   ```bash
   git clone https://github.com/justin-napolitano/ch4-emissions.git
   cd ch4-emissions
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Build the project:
   ```bash
   python python_build.py
   ```
   or manually:
   ```bash
   jupyter-book build jupyter-book
   ```

Check `jupyter-book/_build/html` for reports.

### Gotchas
Ensure you have Python 3.x and pip.
