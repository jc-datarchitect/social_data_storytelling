<div align="center">
  <img src="https://github.com/user-attachments/assets/1cb297c6-2cfd-44ae-bb9e-e385ab79dd69" width="100%" alt="Social Education vs Hate Crimes Cover">

  <h1>Social Education vs. Hate Crimes: An Empirical Analysis in Spain and the EU</h1>

  <p><i>"The outlier is a person"</i></p>
  
  <br>

  [![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/)
  [![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=flat&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
  [![Plotly](https://img.shields.io/badge/Visualization-Plotly-3F4F75?style=flat&logo=plotly&logoColor=white)](https://plotly.com/)
</div>

---

## 🚀 Project Overview

**Social Education vs. Hate Crimes** is an advanced data storytelling and empirical investigation that addresses a profound socio-statistical paradox: *An increase in the historical registry of hate crimes does not necessarily reflect an increase in baseline violence, but rather a higher civic willingness to report incidents*. 

Awarded **"Matrícula de Honor" (Highest Honors, 9.9/10)**, the system systematically blends national law enforcement microdata from Spain with international educational metrics from the OECD (PISA 2022). By leveraging programmatic data pipelines, the project demonstrates how highly educated frameworks and multicultural awareness act as structural catalysts for civil rights defense, shifting the focus from purely descriptive criminal statistics to predictive socio-educational correlations.

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

---

## Data Sources & Reproducibility
Due to GitHub's file size limitations, the primary national security dataset exceeding 100 MB is documented externally to guarantee repository performance while maintaining absolute reproducibility.

1. **Hate Crimes Dataset (`06001.csv`) [160 MB]:**
   * **Source:** *Portal Estadístico de Criminalidad — Ministerio del Interior (Gobierno de España)*. Contains detailed microdata of known hate crime incidents.
   * **Reproducibility Note:** To execute the notebook locally, download the official source file and place it in the `/data` directory with the exact filename `06001.csv`.
2. **Educational Attainment Dataset (`nivfor_1_04.csv`):**
   * **Source:** *Ministerio para la Transformación Digital y de la Función Pública*. Population aged 25–64 in the EU by urbanization degree, gender, and higher education level (2024).
3. **OECD PISA 2022 Dataset (`CY08MSP_SCH_QQQ.SAV`):**
   * **Source:** *Organisation for Economic Co-operation and Development (OECD)*. School questionnaire data evaluating the Multicultural and Social Awareness Index (`DMCVIEWS`).

---

## Data Storytelling & Visualizations
The analytical pipeline follows a structured **Martini Glass narrative architecture**, driving the user from macro-historical trends down to specialized multi-variable correlations.

### Phase 1: The Historical Trend & Anomalies
Using programmatic time-series analysis, this phase maps the evolution of hate crimes in Spain, isolating external sociopolitical shocks.
* **Key Finding:** A clear, continuous upward trajectory peaking significantly in 2023, with a distinct structural drop in 2020 caused by COVID-19 mobility restrictions. This baseline forms the foundation of the reporting paradox.

```text
[INSERT CAPTURE: 01_historical_trend.png]
*Figure 1: Longitudinal evolution of registered hate crimes in Spain (2014-2023).*





