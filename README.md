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

## Repository Architecture

The infrastructure of this repository is strictly organized to ensure computational reproducibility, clean separation of concerns, and immediate access to executive documentation:

```text
├── data/
│   ├── nivfor_1_04.csv                  # EU Educational attainment dataset (Local)
│   └── CY08MSP_SCH_QQQ.SAV              # OECD PISA 2022 School Microdata (SPSS format)
├── notebooks/
│   └── data_storytelling_notebook.ipynb # Production Pipeline (ETL, EDA, Merges, Analytics)
├── documentation/
│   └── data_storytelling_presentation.pptx # Executive Slides & Theoretical Framework
```

---

## Data Sources & Institutional Providers

The production pipeline integrates three official datasets to cross-examine criminal registries against socio-educational frameworks. Below are the technical specifications, storage status, and direct institutional links for reproducibility:

### 1. National Hate Crimes Microdata (Spain)
* **Provider:** *Ministerio del Interior, Gobierno de España – Portal Estadístico de Criminalidad.*
* **Dataset Concept:** Microdata of registered historical incidents classified by discriminatory typologies and geographical distribution.
* **Storage Status:** 🔴 **ACTION REQUIRED (External Download)** — Exceeds GitHub size limits (~160 MB).
* **Filename string in local execution:** `06001.csv` (Must be placed inside the `/data` directory).
* **Official Access Link:** [Portal Estadístico de Criminalidad - Delitos de Odio](https://estadisticasdecriminalidad.ses.mir.es/publico/portalestadistico/datos.html?type=jaxi&title=Delitos%20de%20odio&path=/Datos6/)

### 2. European Educational Attainment Metrics
* **Provider:** *Ministerio para la Transformación Digital y de la Función Pública, Gobierno de España.*
* **Dataset Concept:** Longitudinal metrics mapping European Union populations (ages 25–64) segmented by country, gender, degree level, and urbanization rates.
* **Storage Status:** 🟢 **INCLUDED** — Already tracked in the repository.
* **Filename string:** `data/nivfor_1_04.csv`
* **Official Access Link:** [Datos.gob.es - Población de 25 a 64 años en la UE](https://datos.gob.es/es/catalogo/e05230301-poblacion-de-25-a-64-anos-en-la-ue-por-pais-sexo-nivel-de-formacion-grado-de-urbanizacion-y-ano)

### 3. OECD PISA 2022 School Microdata
* **Provider:** *Organization for Economic Co-operation and Development (OECD).*
* **Dataset Concept:** Global student and institutional background questionnaires, specifically extracted to compute the School Multicultural Awareness Index (`DMCVIEWS`).
* **Storage Status:** 🟢 **INCLUDED** — Already tracked in the repository (SPSS format).
* **Filename string:** `data/CY08MSP_SCH_QQQ.SAV`
* **Official Access Link:** [OECD PISA 2022 Database](https://webfs.oecd.org/pisa2022/index.html)

---

## Phase 1: National Hate Crime Dynamics (2014–2024)

This initial analytical phase dissects a decade of raw institutional records from Spain’s Ministry of the Interior. Instead of reading these metrics as a simple volume of violence, the data pipeline uncovers a complex sociostatistical behavior driven by institutional transparency, legislative updates, and reporting willingness.

---

### 1. Recent Evolution of a Persistent Phenomenon

A longitudinal overview of total registered incidents establishes the foundational baseline of the paradox: a steady upward trajectory in raw data, interrupted only by global macroeconomic anomalies.

<div align="center">
  <img src="https://github.com/user-attachments/assets/9c7167ab-4eaf-45a7-9ca5-b35a4598fc69" width="100%" alt="Evolución Anual de los Delitos de Odio en España">
</div>

* **Structural Upward Trend:** Registered incidents exhibit an unbroken growth trajectory since 2014, showing that the phenomenon has gained massive statistical visibility over the last decade.
* **The 2020 Pandemic Anomaly:** A sharp, temporary drop occurs in 2020. This systemic deceleration directly correlates with COVID-19 mobility restrictions, lockdowns, and the temporary suppression of public and physical social interactions.
* **Historical Peak (2023):** The registry reaches its absolute historical maximum in 2023 with 2,268 cases. This milestone underpins the core thesis: greater civic awareness and streamlined institutional reporting channels actively pull hidden incidents out of the *cifra negra* (underreporting).

---

### 2. Hate is Not Homogeneous

Breaking down the aggregate metrics into specific discriminatory typologies reveals that the drivers behind these records are heavily stratified.

<div align="center">
  <img src="https://github.com/user-attachments/assets/cea638bc-af60-40a8-8af1-a4511a3d6c75" width="100%" alt="Distribución por Tipología de Delitos de Odio">
</div>

* **Dominance of Racism and Xenophobia:** This typology consistently concentrates the highest absolute volume of hate crimes throughout the entire decade, reinforcing its place as the primary frontier for social intervention.
* **Sustained Growth in LGBTQI+ Discrimination:** Incidents tied to sexual orientation and gender identity display an aggressive and steady percentage increase, marking a profound shift in victims' willingness to report offenses to law enforcement.
* **Multi-Dynamic Overlap:** The overall national increase is not caused by a single uniform factor, but rather by the simultaneous overlap of multiple distinct social dynamics running on different tracks.

---

### 3. Not All Forms of Hate Evolve Similarly

A direct comparison between the endpoints of the decade (2014 vs. 2024) isolates the exact velocity and direction of each independent typology.

<div align="center">
  <img src="https://github.com/user-attachments/assets/45f2249f-42e4-4f2d-9ff7-65d4b1c0bd79" width="100%" alt="Diferencia en Incidentes de Odio: 2014 vs 2024">
</div>

* **Asymmetric Absolute Growth:** Racism and xenophobia lead the decade's increase with an absolute growth of +380 incidents, cementing its status as the most statistically expansive category.
* **Emergence of Specific Vectors:** Gender-based discrimination (+188) and ideological motives (+152) showcase significant upward shifts, reflecting how legislative frameworks and social awareness have successfully formalized these definitions over time.
* **Divergent Trajectories:** While most categories expand, certain typologies display moderate stagnation or isolated drops (such as disability-related crimes or religious beliefs), demonstrating that independent social contexts drive different forms of hate.

---

### 4. Territorial Incidence of Hate

Mapping the geographic density of registered incidents transitions the analysis from a temporal dimension to a spatial framework, identifying key regional hotspots.

<div align="center">
  <img src="https://github.com/user-attachments/assets/156b47ef-d101-4022-bbe0-c9c116207edd" width="100%" alt="Distribución Geográfica de Delitos de Odio">
</div>

* **Geographical Clustering:** The relative incidence rate per 100,000 inhabitants exposes significant territorial disparities, identifying clear regional clusters with higher concentrations of registered cases (such as the Basque Country and Navarre).
* **Socio-Contextual Catalysts:** These regional variances do not automatically imply a higher baseline of structural hatred in those areas. Instead, they reflect the presence of localized social variables, highly active regional victim-support networks, and variations in law enforcement training regarding hate crime identification.

---



---


---

## Data Storytelling & Visualizations
The analytical pipeline follows a structured **Martini Glass narrative architecture**, driving the user from macro-historical trends down to specialized multi-variable correlations.

### Phase 1: The Historical Trend & Anomalies
Using programmatic time-series analysis, this phase maps the evolution of hate crimes in Spain, isolating external sociopolitical shocks.
* **Key Finding:** A clear, continuous upward trajectory peaking significantly in 2023, with a distinct structural drop in 2020 caused by COVID-19 mobility restrictions. This baseline forms the foundation of the reporting paradox.

```text
[INSERT CAPTURE: 01_historical_trend.png]
*Figure 1: Longitudinal evolution of registered hate crimes in Spain (2014-2023).*





