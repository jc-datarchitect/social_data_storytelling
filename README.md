<div align="center">
  <img src="https://github.com/user-attachments/assets/6b5142c7-e39e-43ca-8cb6-58c7b39ce11e" width="100%" alt="Social Education vs Hate Crimes Cover">

<h1>Can Education Prevent Hate?<br>Hate Crimes, Education, and Tolerance: A Data-Driven Reading</h1>

  <br>

  [![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/)
  [![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=flat&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
  [![Plotly](https://img.shields.io/badge/Visualization-Plotly-3F4F75?style=flat&logo=plotly&logoColor=white)](https://plotly.com/)
</div>

---

## Project Overview

**Can Education Prevent Hate?** is an empirical data science investigation and strategic data storytelling framework developed as a Master's Final Project and awarded **"Matrícula de Honor" (Highest Honors, 9.9/10)**. The investigation is designed to confront a significant socio-statistical paradox: *an ongoing statistical increase in the historical registry of hate crimes does not necessarily denote a rise in structural violence, but rather a profound shift in civic willingness to identify and report incidents.*

By building a programmatic data pipeline that blends a decade of complex law enforcement microdata from Spain with international educational attainment metrics and secondary school environment benchmarks (OECD-PISA 2022), this repository moves past purely descriptive criminal metrics. Instead, it establishes an analytical narrative demonstrating how highly educated frameworks and multicultural awareness act as structural catalysts for civil rights defense, successfully mitigating underreporting (*cifra negra*) and shifting the focus toward predictive socio-educational correlations.

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





