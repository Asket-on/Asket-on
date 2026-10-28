# Mikhail Volobuev

**Data Engineer** with 8+ years of enterprise domain experience in **Banking Risk & Financial Analytics** (Sberbank, VTB).  
Specializing in modern cloud data warehouses (**Google Cloud BigQuery**, **PostgreSQL**), modular transformation & modeling (**dbt Core**, Data Vault 2.0, SCD), and containerised batch & streaming pipelines (**Apache Airflow**, **PySpark**, **Kafka**).

- 📍 **Location**: Bochum, North Rhine-Westphalia (NRW), Germany (Open to on-site, hybrid & remote roles across Germany)
- 💼 **Domain Background**: Credit risk modeling, financial analytics & data reconciliation since 2016; Data Engineering specialized since selective training at Sberbank Corporate University (2019–2020).
- 📜 **Credentials**: *Google Cloud Data Engineering Professional Certificate (Coursera)* | Yandex Practicum Data Engineering Specialization.
- 📬 **Contact**: [LinkedIn](https://www.linkedin.com/in/mik-volo/) | [Email](mailto:mvolobuev@gmail.com) | [Telegram](https://t.me/Asket_on)

---

## Featured Flagship Project

### [de-financial-dwh-pipeline](https://github.com/Asket-on/de-financial-dwh-pipeline)
[![CI](https://github.com/Asket-on/de-financial-dwh-pipeline/actions/workflows/ci.yml/badge.svg)](https://github.com/Asket-on/de-financial-dwh-pipeline/actions/workflows/ci.yml)
[![Pages](https://github.com/Asket-on/de-financial-dwh-pipeline/actions/workflows/pages.yml/badge.svg)](https://asket-on.github.io/de-financial-dwh-pipeline/)
[![Release](https://img.shields.io/badge/release-v1.1.1-blue.svg)](https://github.com/Asket-on/de-financial-dwh-pipeline/releases/tag/v1.1.1)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/Asket-on/de-financial-dwh-pipeline/blob/main/LICENSE)

A reproducible, multi-target financial data warehouse demo demonstrating batch ELT across three storage tiers, designed from real-world banking domain experience:
- **Tier 1 (Zero-Dependency Local)**: Python standard library + SQLite — executes instantly without infrastructure overhead.
- **Tier 2 (Enterprise Containerized)**: PostgreSQL with dedicated `staging` and `dwh` schemas, orchestrated via Apache Airflow with verified bounded catchup.
- **Tier 3 (Modern Cloud Scale)**: **Google Cloud BigQuery & GCS** featuring partitioning (`PARTITION BY DATE`), clustering (`CLUSTER BY currency_code, status`), deterministic `QUALIFY` deduplication, and in-warehouse machine learning (`ARIMA_PLUS` 7-day volume forecasting via BigQuery ML).
- **Data Quality & Integrity**: 5/5 SQL quality assertions enforcing FX-rate completeness, grain preservation, join-fanout protection, and non-null constraints. 26/26 unit tests in automated GitHub Actions CI.

🔗 **Live Dashboard:** [asket-on.github.io/de-financial-dwh-pipeline](https://asket-on.github.io/de-financial-dwh-pipeline/)  
📖 **Architecture Guide:** [BigQuery Cloud Warehouse Architecture](https://github.com/Asket-on/de-financial-dwh-pipeline/blob/main/docs/bigquery_architecture.md)

---

## Technology Stack

<table>
  <tr>
    <td valign="top" width="50%">
      <h3>⚙️ Data Engineering & Cloud</h3>
      <ul>
        <li><b>Cloud & DWH:</b> Google Cloud Platform (BigQuery, Cloud Storage, BigQuery ML), PostgreSQL, ClickHouse, Vertica</li>
        <li><b>Transformation & Modeling:</b> dbt Core, Dimensional Modeling (Star / Snowflake), Data Vault 2.0, Slowly Changing Dimensions (SCD)</li>
        <li><b>Orchestration & CI/CD:</b> Apache Airflow, Docker, Docker Compose, GitHub Actions, Linux/Bash</li>
        <li><b>Streaming & Big Data:</b> Apache Spark (PySpark, Structured Streaming), Apache Kafka, Redis</li>
        <li><b>Languages & Querying:</b> Python 3.10+, SQL (BigQuery, PostgreSQL, SQLite, Vertica ANSI SQL)</li>
      </ul>
    </td>
    <td valign="top" width="50%">
      <h3>📊 Financial Analytics & Applied ML</h3>
      <ul>
        <li><b>Domain Analytics:</b> Corporate credit risk evaluation, DCF modeling, transaction reconciliation, audit trail validation</li>
        <li><b>Data Science & ML:</b> PyTorch, Scikit-Learn, LightGBM, Pandas, NumPy, BigQuery ML</li>
        <li><b>Visualisation & BI:</b> Metabase, Power BI, Looker Studio, GitHub Pages reports</li>
        <li><b>Engineering Standards:</b> Automated Data Quality gates (WAP pattern), deterministic sampling, Clean Code, test-driven validation</li>
      </ul>
    </td>
  </tr>
</table>

---

## Selected Projects

### 🎬 [imdb-movie-analysis-dwh](https://github.com/Asket-on/imdb-movie-analysis-dwh)
*An automated analytical warehouse pipeline utilizing **dbt Core**, **PostgreSQL**, and **Apache Airflow**:*
- Implemented modular 3-layer dbt modeling (`staging` $\rightarrow$ `intermediate` $\rightarrow$ `marts`) parsing multi-million record compressed TSV archives.
- Automated generic and custom dbt Data Quality assertions enforcing primary key uniqueness, referential integrity, and runtime constraints.
- Integrated Docker Compose orchestration running PostgreSQL 15 and Airflow with idempotent DAG task definitions.

### 🚀 [Data Engineering Projects](https://github.com/Asket-on/Data_engineer_projects)
*A collection of 9 containerised data engineering pipelines developed during the Yandex Practicum specialization and systematically refactored for reproducibility:*
- **Real-Time Spark Streaming**: Kafka stream-static joins with PostgreSQL metadata tables in PySpark.
- **Microservices & Kafka Streaming**: Microservice stream-processing pipeline using Kafka, Redis dictionary cache, PostgreSQL, and Docker.
- **Community Conversion Data Vault**: Analytical DWH modeled in **Data Vault 2.0** (Hubs, Links, Satellites).
- **Slowly Changing Dimensions**: Incremental Airflow ETL pipeline parsing MongoDB order payloads into SCD Format.

### 🦅 [Bird Strike & Weather Pipeline](https://github.com/Asket-on/bird-strike-weather-pipeline)
*An ETL data enrichment pipeline with automated Data Quality circuit breakers:*
- Enriches aviation incident logs with historical meteorological observations via Open-Meteo multi-coordinate batch API.
- Implements Write-Audit-Publish (WAP) Data Quality checks (`dq.py`) and zero-dependency standard library architecture with Docker and Airflow orchestration.

### 🎵 [Album Cover Genre Classification](https://github.com/Asket-on/album-cover-genre-classification)
*A Computer Vision & Deep Learning pipeline for audio-visual alignment:*
- Multi-label audio genre and mood classification directly from album cover artwork using PyTorch and pre-trained CNN backbones (ResNet, ConvNeXt).

---

## 🇩🇪 Über mich / Standort

- **Standort:** Bochum, Nordrhein-Westfalen (NRW), Deutschland (Offen für Vor-Ort, Hybrid & Remote Positionen deutschlandweit)
- **Sprachen:**
  - **Englisch:** Verhandlungssicheres technisches Verständnis (Lesen und Verfassen von Spezifikationen, Architekturdokumenten, RFCs & asynchrone Ticket-/PR-Kommunikation; mündliche Grundkenntnisse)
  - **Deutsch:** DTZ B1 zertifiziert (Technisches Verständnis, Dokumentation & tägliche Team-Kollaboration; mündliche Grundkenntnisse)
  - **Russisch:** Muttersprache
- **Schwerpunkte:** Data Platform Engineering, Cloud DWH (BigQuery, PostgreSQL), dbt Core, skalierbare Batch- & Streaming-Pipelines (Airflow, PySpark, Kafka), Data Quality Engineering

---

## 📊 GitHub Analytics

<p align="left">
  <img src="https://github-readme-stats.vercel.app/api?username=Asket-on&show_icons=true&theme=nord&count_private=true" alt="Asket-on GitHub Stats" height="150" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Asket-on&layout=compact&theme=nord&hide=jupyter,html,css" alt="Asket-on Top Languages" height="150" />
</p>
