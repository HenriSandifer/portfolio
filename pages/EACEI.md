[🏠 HOME](../README.md)
[🇫🇷 Version française](EACEI_FR.md)
[🇮🇹 Versione Italiana](EACEI_IT.md)

# 🏭 EACEI - French Industrial Energy Consumption Analysis

**Author**: [Henri Sandifer](https://github.com/henrisandifer)

![Dashboard Screenshot](../assets/eacei.png)

### 👉🌐 View the **Live Dashboard** : [Power BI Dashboard](https://app.powerbi.com/view?r=eyJrIjoiZTE4YjVhMjctZjFmZS00YjRjLThlOTctNDAyOGI0ZTNiNGNiIiwidCI6ImJlOTNmMTc4LTA5NjQtNDcwOS1hMDZjLTY4ZThhZjBhODM1NSJ9&pageName=f779d68dcac6fc795d20)

---

## 📺 Video presentation
<!-- [![Video presentation](https://img.youtube.com/vi/AsAM7ZAL63o/0.jpg)](https://youtu.be/AsAM7ZAL63o?si=KiCLegoh95UAntpA)-->
### ⌛ Coming soon

---

## 1. Project Overview

This project aims to analyze the annual survey on energy consumption in French industry (_Enquête Annuelle sur la Consommation d'Énergie dans l'Industrie_ - **EACEI**), published by INSEE.  
The primary goal is to build a robust, end-to-end data pipeline to clean, transform, and model over a decade's worth of data (2010–2023).

The final output is a clean, relational database (star schema) and an interactive dashboard designed to explore trends in energy consumption across different industrial sectors, regions, and company sizes.

This project demonstrates skills in:

- Data cleaning
- ETL (Extract, Transform, Load)
- Database design
- Data visualization

---

## 2. Data Source

- **Provider**: INSEE (_Institut national de la statistique et des études économiques_)
- **Dataset**: EACEI
- **Years**: 2010–2023
- **Link**: [\[INSEE data source page (2023)\]](https://www.insee.fr/fr/statistiques/8566228?sommaire=8566231)

> The raw data consists of 156 individual CSV files, initially downloaded in .xls and .xlsx format from the individual EACEI pages for each year, with significant variations in structure, naming conventions, and categorical codes over the years.

---

## 3. Project Architecture

To handle the complexity and enable powerful analytics, this project uses a classic **Star Schema** database design.  
This separates the core measurements (facts) from their descriptive attributes (dimensions), leading to a clean, efficient, and scalable model.

- **Fact Table**: `faits_eacei`  
  → Contains all numerical values (consumption, purchases, prices, etc.)

- **Dimension Tables**:
  - `dim_naf`
  - `dim_reg`
  - `dim_teff`
  - `dim_ind`
  - `dim_year`

---

## 4. The Data Pipeline

The project is structured as a sequential pipeline, with scripts organized into phases:

### Phase 0 – Setup

- Initialization of the project structure and version control.

### Phase 1 – Cleaning & Standardization

- Process raw CSVs from `00_data_raw/`.
- Fuse headers, aggregate columns/rows to match modern conventions.
- Output tidy "wide" tables to `01_data_clean/`.

### Phase 2 – Dimension Generation

- Extract unique attributes.
- Generate primary keys.
- Output dimension tables to `03_database_final/`.

### Phase 3 – Fact Table Assembly

- Melt wide tables to long format.
- Join dimension table IDs to create `faits_eacei.csv`.

### Phase 4 – Visualization

- Load final tables into a BI tool for interactive dashboarding.

---

## 5. Tools & Technologies

- **Language**: Python 3.13
- **Libraries**: Pandas, NumPy
- **Database**: MySQL, Star-schema
- **Visualization**: Power BI
- **Version Control**: Git & GitHub

---

## 6. Current Status & Next Steps

- [✔️] Phase 1: Standardize all 164 raw CSV files
- [✔️] Phase 2: Generate all dimension tables
- [✔️] Phase 3: Build the final fact table
- [✔️] Phase 4: Design and build the interactive dashboard
