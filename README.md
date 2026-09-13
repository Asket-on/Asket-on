# Hi, I'm Mikhail Volobuev 👋
### Data Engineer & Data Scientist | Architecting Scalable Pipelines & Cloud DWH

I specialize in building robust, end-to-end data architectures, processing high-throughput streaming and batch data, and deploying production-ready analytical pipelines. My focus is on data reliability, performance optimization, and clean warehouse modeling.

- 🔭 **Current Focus**: Modern Cloud DWH (Google Cloud BigQuery & GCS), stream-table joins with PySpark, and enterprise Airflow orchestration.
- ⚙️ **Engineering Principles**: Complete containerisation, strict idempotency guarantees, visible data-quality gates, and clean, decoupled architectures.
- 📜 **Credentials**: *Google Cloud Professional Certificate: Cloud Data Engineer* | Yandex Practicum Data Engineering & Data Science specializations.

---

## 🏗️ Featured Flagship Project

### 🌟 [de-financial-dwh-pipeline](https://github.com/Asket-on/de-financial-dwh-pipeline)
[![CI](https://github.com/Asket-on/de-financial-dwh-pipeline/actions/workflows/ci.yml/badge.svg)](https://github.com/Asket-on/de-financial-dwh-pipeline/actions/workflows/ci.yml)
[![Pages](https://github.com/Asket-on/de-financial-dwh-pipeline/actions/workflows/pages.yml/badge.svg)](https://asket-on.github.io/de-financial-dwh-pipeline/)
[![Release](https://img.shields.io/badge/release-v1.1.1-blue.svg)](https://github.com/Asket-on/de-financial-dwh-pipeline/releases/tag/v1.1.1)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/Asket-on/de-financial-dwh-pipeline/blob/main/LICENSE)

A production-grade, multi-target financial data warehouse pipeline demonstrating batch ELT across three storage tiers:
- **Tier 1 (Zero-Dependency Local)**: Python standard library + SQLite — runs instantly in seconds without setup overhead.
- **Tier 2 (Enterprise Containerized)**: PostgreSQL with separate `staging` and `dwh` schemas, orchestrated by Airflow with verified bounded catchup.
- **Tier 3 (Modern Cloud Scale)**: **Google Cloud BigQuery & GCS** featuring partition (`PARTITION BY DATE`) and clustering (`CLUSTER BY currency_code, status`) cost optimization, deterministic `QUALIFY` deduplication, and in-warehouse machine learning (`ARIMA_PLUS` 7-day volume forecasting via BigQuery ML).
- **Quality & Assurance**: 5/5 SQL quality assertions protecting against corrupt amounts, missing exchange rates, duplicate grain, and join fanouts. 24/24 passing unit tests in automated GitHub Actions CI.

🔗 **Live Dashboard:** [asket-on.github.io/de-financial-dwh-pipeline](https://asket-on.github.io/de-financial-dwh-pipeline/)  
📖 **Architecture Guide:** [BigQuery Cloud Warehouse Architecture](https://github.com/Asket-on/de-financial-dwh-pipeline/blob/main/docs/bigquery_architecture.md)

---

## 🛠️ Technology Stack

<table>
  <tr>
    <td valign="top" width="50%">
      <h3>⚙️ Data Engineering & Cloud</h3>
      <ul>
        <li><b>Cloud & DWH:</b> Google Cloud Platform (BigQuery, Cloud Storage, BigQuery ML), ClickHouse, PostgreSQL, Vertica, Hadoop</li>
        <li><b>Orchestration & CI:</b> Apache Airflow, Docker, Docker Compose, GitHub Actions</li>
        <li><b>Stream & Big Data:</b> Apache Spark (PySpark, Structured Streaming), Apache Kafka</li>
        <li><b>Databases & Caches:</b> PostgreSQL, Redis, MongoDB, MySQL, SQLite</li>
        <li><b>Languages & Tools:</b> Python (Advanced), SQL (BigQuery, PostgreSQL, SQLite), Bash</li>
      </ul>
    </td>
    <td valign="top" width="50%">
      <h3>📊 Data Science & Machine Learning</h3>
      <ul>
        <li><b>ML Frameworks:</b> PyTorch, Scikit-Learn, LightGBM, XGBoost, BigQuery ML</li>
        <li><b>Data Analysis:</b> Pandas, NumPy, SciPy, Matplotlib, Seaborn</li>
        <li><b>Computer Vision:</b> OpenCV, PIL, Torchvision (ResNet, ConvNeXt)</li>
        <li><b>MLOps & API:</b> FastAPI, Flask, MLflow</li>
        <li><b>Visualisation:</b> Metabase, Tableau, Looker Studio, Jupyter</li>
      </ul>
    </td>
  </tr>
</table>

---

## 📁 More Portfolio Highlights

### 🚀 [Data Engineering Projects](https://github.com/Asket-on/Data_engineer_projects)
*A comprehensive collection of 9 production-grade data engineering pipelines, systematically refactored and containerised:*
- **Project 9 (Financial DWH Pipeline)**: Scheduled batch pipeline with exchange-rate deduplication and analytical mart metrics in `dwh.global_metrics`.
- **Project 8 (Cloud Streaming DWH)**: Microservice-driven streaming pipeline using Kafka, Redis dictionary cache, PostgreSQL, and Docker.
- **Project 7 (Real-Time Spark Streaming)**: Real-time user event stream-static joins from Kafka with Postgres metadata tables in PySpark.
- **Project 5 (Community Conversion Data Vault)**: Analytical DWH implemented in **Data Vault 2.0** model (Hubs, Links, Satellites).
- **Project 4 (Slowly Changing Dimensions)**: Incremental Airflow ETL pipeline parsing MongoDB order payloads and compiling courier metrics in SCD Format.

### 🎵 [Yandex Music Cover Detection](https://github.com/Asket-on/yandex_music_cover_detection)
*A Machine Learning / Computer Vision pipeline for audio-visual alignment:*
- Developed deep learning models to predict audio genre, mood, and artist metadata directly from album cover graphics.
- Utilized PyTorch and pre-trained ResNet/ConvNeXt backbones with custom multi-label classification heads.

### 🦅 [Bird Strike & Weather Pipeline](https://github.com/Asket-on/bird-strike-weather-pipeline)
*An ETL data enrichment pipeline connecting aviation incident logs with weather data:*
- Fetches real-time weather logs from global meteorological APIs matching the date and location coordinates of aviation bird strike events.
- Performs cleaning, deduplication, and stores enriched datasets in an analytical database for risk analysis.

---

## 📊 GitHub Analytics

<p align="left">
  <img src="https://github-readme-stats.vercel.app/api?username=Asket-on&show_icons=true&theme=nord&count_private=true" alt="Asket-on GitHub Stats" height="150" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Asket-on&layout=compact&theme=nord&hide=jupyter,html,css" alt="Asket-on Top Languages" height="150" />
</p>

---

## 📈 Activity & Streak

<p align="left">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=Asket-on&theme=nord" alt="Asket-on Commit Streak" height="150" />
</p>
