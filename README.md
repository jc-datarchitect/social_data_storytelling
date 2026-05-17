# Social Education vs. Hate Crimes: An Empirical Analysis in Spain and the EU
**Javier Cristóbal — Architect & Data Scientist**

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-2.0+-darkblue.svg)](https://pandas.pydata.org/)
[![Plotly](https://img.shields.io/badge/Plotly-Interactive-purple.svg)](https://plotly.com/)

---

## Executive Summary & The Analytical Paradox
This project delivers a comprehensive data storytelling narrative investigating the relationship between educational frameworks, social awareness, and the reporting rates of hate crimes across Spain and the European Union. Funded on rigorous statistical exploration, this work was awarded **"Matrícula de Honor" (Highest Honors, 9.9/10)**.

The core of this investigation tackles a profound socio-statistical paradox: **An increase in the historical registry of hate crimes does not necessarily reflect an increase in violence, but rather a higher civic willingness to report incidents, heavily driven by social education, multi-cultural awareness, and institutional trust.** By blending national law enforcement data with international education metrics (OECD-PISA), this project moves from descriptive statistics to predictive correlation analysis.

---

## Project Architecture
The repository is strictly structured to separate raw data infrastructure, reproducible computation, and executive documentation:

```text
├── data/
│   ├── nivfor_1_04.csv          # EU Educational attainment dataset (Local)
│   └── CY08MSP_SCH_QQQ.SAV      # OECD PISA 2022 School Questionnaire (Local)
├── notebooks/
│   └── data_storytelling_notebook.ipynb  # Comprehensive production Pipeline
└── documentation/
    └── data_storytelling_presentation.pptx      # Executive Slides & Theoretical Framework
