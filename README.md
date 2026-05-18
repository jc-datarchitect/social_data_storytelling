<div align="center">
  <img src="https://github.com/user-attachments/assets/6b5142c7-e39e-43ca-8cb6-58c7b39ce11e" width="100%" alt="Social Education vs Hate Crimes Cover">

<h1>Can Education Prevent Hate?<br>Hate Crimes, Education, and Tolerance: A Data-Driven Reading</h1>

  <br>

  [![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/)
  [![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=flat&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
  [![Plotly](https://img.shields.io/badge/Visualization-Plotly-3F4F75?style=flat&logo=plotly&logoColor=white)](https://plotly.com/)
  [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg?style=flat)](https://opensource.org/licenses/MIT)
  [![GitHub stars](https://img.shields.io/github/stars/jc-datarchitect/TRIP-U?style=social)](https://github.com/jc-datarchitect/TRIP-U/stargazers)
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

## Execution & Local Deployment

To run the complete ETL, data blending, and predictive visualizations locally inside the production pipeline:

1. Clone this repository locally.
2. Ensure you download the national criminal microdata file manually as specified in the [Data Sources](#-data-sources--institutional-providers) section due to file size limitations.
3. Launch your local environment and execute the notebook: `notebooks/data_storytelling_notebook.ipynb`.

---

## Phase 1: National Hate Crime Dynamics (2014–2024)

This initial analytical phase dissects a decade of raw institutional records from Spain’s Ministry of the Interior. Instead of reading these metrics as a simple volume of violence, the data pipeline uncovers a complex sociostatistical behavior driven by institutional transparency, legislative updates, and reporting willingness.

---

### 1.1. Recent Evolution of a Persistent Phenomenon

A longitudinal overview of total registered incidents establishes the foundational baseline of the paradox: a steady upward trajectory in raw data, interrupted only by global macroeconomic anomalies.

<div align="center">
  <img src="https://github.com/user-attachments/assets/9c7167ab-4eaf-45a7-9ca5-b35a4598fc69" width="100%" alt="Evolución Anual de los Delitos de Odio en España">
</div>

* **Structural Upward Trend:** Registered incidents exhibit an unbroken growth trajectory since 2014, showing that the phenomenon has gained massive statistical visibility over the last decade.
* **The 2020 Pandemic Anomaly:** A sharp, temporary drop occurs in 2020. This systemic deceleration directly correlates with COVID-19 mobility restrictions, lockdowns, and the temporary suppression of public and physical social interactions.
* **Historical Peak (2023):** The registry reaches its absolute historical maximum in 2023 with 2,268 cases. This milestone underpins the core thesis: greater civic awareness and streamlined institutional reporting channels actively pull hidden incidents out of the *cifra negra* (underreporting).

---

### 1.2. Hate is Not Homogeneous

Breaking down the aggregate metrics into specific discriminatory typologies reveals that the drivers behind these records are heavily stratified.

<div align="center">
  <img src="https://github.com/user-attachments/assets/cea638bc-af60-40a8-8af1-a4511a3d6c75" width="100%" alt="Distribución por Tipología de Delitos de Odio">
</div>

* **Dominance of Racism and Xenophobia:** This typology consistently concentrates the highest absolute volume of hate crimes throughout the entire decade, reinforcing its place as the primary frontier for social intervention.
* **Sustained Growth in LGBTQI+ Discrimination:** Incidents tied to sexual orientation and gender identity display an aggressive and steady percentage increase, marking a profound shift in victims' willingness to report offenses to law enforcement.
* **Multi-Dynamic Overlap:** The overall national increase is not caused by a single uniform factor, but rather by the simultaneous overlap of multiple distinct social dynamics running on different tracks.

---

### 1.3. Not All Forms of Hate Evolve Similarly

A direct comparison between the endpoints of the decade (2014 vs. 2024) isolates the exact velocity and direction of each independent typology.

<div align="center">
  <img src="https://github.com/user-attachments/assets/45f2249f-42e4-4f2d-9ff7-65d4b1c0bd79" width="100%" alt="Diferencia en Incidentes de Odio: 2014 vs 2024">
</div>

* **Asymmetric Absolute Growth:** Racism and xenophobia lead the decade's increase with an absolute growth of +380 incidents, cementing its status as the most statistically expansive category.
* **Emergence of Specific Vectors:** Gender-based discrimination (+188) and ideological motives (+152) showcase significant upward shifts, reflecting how legislative frameworks and social awareness have successfully formalized these definitions over time.
* **Divergent Trajectories:** While most categories expand, certain typologies display moderate stagnation or isolated drops (such as disability-related crimes or religious beliefs), demonstrating that independent social contexts drive different forms of hate.

---

### 1.4. Territorial Incidence of Hate

Mapping the geographic density of registered incidents transitions the analysis from a temporal dimension to a spatial framework, identifying key regional hotspots.

<div align="center">
  <img src="https://github.com/user-attachments/assets/156b47ef-d101-4022-bbe0-c9c116207edd" width="100%" alt="Distribución Geográfica de Delitos de Odio">
</div>

* **Geographical Clustering:** The relative incidence rate per 100,000 inhabitants exposes significant territorial disparities, identifying clear regional clusters with higher concentrations of registered cases (such as the Basque Country and Navarre).
* **Socio-Contextual Catalysts:** These regional variances do not automatically imply a higher baseline of structural hatred in those areas. Instead, they reflect the presence of localized social variables, highly active regional victim-support networks, and variations in law enforcement training regarding hate crime identification.

---

---

## Phase 2: Socio-Educational Mapping & The European Context

To interpret the structural rise in reported hate crimes, the analytical pipeline pivots from penal metrics to regional educational foundations, positioning Spain within the broader European framework. This phase contrasts traditional educational attainment against active institutional and multicultural awareness.

<div align="center">
  <img src="https://github.com/user-attachments/assets/7055d876-bf19-42da-b523-d02e07237f48" width="75%" alt="Socio-Educational Context Pivot">
</div>

---

### 2.1. Spain in the European Educational Landscape

A comparative analysis of tertiary educational attainment across the European Union establishes Spain's baseline structural asset.

<div align="center">
  <img src="https://github.com/user-attachments/assets/303c3ba9-d786-4ffa-aa01-23d0dea0e7e4" width="100%" alt="Proporción del Nivel Educativo Superior en España">
</div>

* **Above-Average Educational Capital:** Spain significantly surpasses the European Union baseline, with **42.0%** of its population (ages 25–64) holding a higher education degree compared to the EU average of **36.1%** (+5.9% advantage).
* **Strategic Social Asset:** This high concentration of educational capital represents a powerful, pre-existing infrastructure capable of driving civic transformation and human rights advocacy.
* **A Lever for Intervention:** Rather than a passive academic metric, this widespread educational foundation functions as a highly practical lever for structural intervention against discriminatory frameworks.

---

### 2.2. Spain and the Cross-Cultural Awareness Benchmark

Transitioning from formal degrees to institutional environments, this section utilizes secondary school microdata to measure active multicultural empathy.

<div align="center">
  <img src="https://github.com/user-attachments/assets/ce94e4da-aea5-416f-b4d9-604c2ffc0e1e" width="100%" alt="Conciencia Social y Multicultural en Centros Educativos - PISA 2022">
</div>

* **The Zero-Baseline Benchmark:** The 0-axis represents the standardized OECD baseline, serving as a clean reference point to divide positive and negative regional deviations.
* **Strong Multicultural Outlook:** Spain ranks clearly above the international average with an index score of **+0.17**, demonstrating a resilient institutional framework for diversity training and social empathy in its formative stages.
* **Pronounced European Asymmetry:** The European landscape displays high volatility, ranging from exceptionally high indices (Portugal at +0.35, Malta at +0.29) to severe negative trends in other Member States, proving that social awareness is heavily localized.

---

### 2.3. The Socio-Educational Matrix: Capital vs. Awareness

By merging both distinct metrics into a four-quadrant matrix, the data pipeline uncovers the directional behavior connecting educational investments with human rights reporting.

<div align="center">
  <img src="https://github.com/user-attachments/assets/33635a12-1f98-418c-a4e8-7d5bb5f087b3" width="100%" alt="Relación entre Proporción de Educación Superior y Conciencia Social">
</div>

* **The Four-Quadrant Heterogeneity:** European countries scatter across four distinct quadrants, confirming that formal tertiary education rates do not automatically guarantee high multicultural awareness on their own.
* **Spain's Virtuous Positioning:** Spain positions itself securely inside the **upper-right quadrant (High Higher Education % / High Social Awareness)**. This critical location explains the reporting paradox: its population is uniquely equipped with both the cognitive tools and the civic empathy necessary to identify, reject, and report hate-driven violations.
* **Deconstructing Hidden Violations:** This layout reinforces the central thesis that a higher registry of hate crimes in highly educated regions is a direct consequence of a robust civic culture dismantling underreporting (*cifra negra*), rather than an increase in real structural violence.

---

## Phase 3: The Behavioral Mechanism & Executive Conclusions

To finalize the statistical narrative, the analysis bridges macro-demographics with institutional actions. This phase formalizes the reporting mechanism and delivers the empirical conclusions of the investigation.

<div align="center">
  <img src="https://github.com/user-attachments/assets/e330b4f6-8345-4ef0-ab2e-159cc6db89ac" width="100%" alt="The Socio-Institutional Data Mechanism">
</div>

* **The Social Dimension:** Structural hate and everyday conflicts organically scale into explicit discriminatory behaviors within public and private spaces.
* **The Socio-Educational Catalyst:** Highly educated frameworks and active multicultural awareness do not reduce the presence of conflict; instead, they function as cognitive lenses that help citizens identify micro-aggressions.
* **The Institutional Outcome:** This heightened civic capacity directly triggers formal reporting and legal classification, expanding the statistical registry to expose problems that previously remained hidden (*cifra negra*).

---

### Key Empirical Findings

The empirical integration of law enforcement data and international educational benchmarks establishes three definitive conclusions:

<div align="center">
  <img src="https://github.com/user-attachments/assets/d36d720a-b983-4467-b26d-8f45b7d1f174" width="100%" alt="Executive Analytical Conclusions">
</div>

1. **Visibility Over Violence:** An expanding historical registry of hate crimes does not necessarily confirm an increase in structural violence. Instead, it reflects a profound shift in civic willingness to identify, reject, and report incidents.
2. **Education Demolishes Underreporting:** Robust socio-educational ecosystems and multicultural awareness act as primary catalysts for reporting, successfully pulling hidden crimes out of historical invisibility and bringing them into official registries.
3. **The Hidden Bias of Low Registries:** Conversely, regions displaying exceptionally low reporting rates or stagnant trends do not guarantee a safer social environment. Instead, they often mask severe institutional underreporting, structural barriers, or systemic marginalization.

---

### Final Reflection: Humanizing the Data

Statistical models, regression analysis, and behavioral matrices provide necessary frameworks to analyze systemic trends. However, predictive data science must maintain its ethical foundation when assessing human conflict.

<div align="center">
  <img src="https://github.com/user-attachments/assets/60c619b9-b3ef-479e-a12b-08518375da15" width="100%" alt="An Outlier is Also a Person">
</div>

> **"The outlier is also a person. Data explains trends, but it does not justify hate."**
>
> Every data point representing a registered incident contains an individual story of discrimination. The ultimate purpose of leveraging big data and analytics within sociological frameworks is not merely descriptive; it is a strategic tool to build actionable equity, optimize protective public policies, and protect civil rights.

---

### Data for Impact & Social Awareness

This repository leverages data science to shed light on hate crimes and explore how education acts as a critical driver for social change. If these insights, exploratory data analysis (EDA), or visualizations helped you better understand this reality (or inspired you not to look away) **consider supporting the project with a ⭐**.

Let's use data to build a more conscious, empathetic, and inclusive society. Feel free to reach out for collaboration!



