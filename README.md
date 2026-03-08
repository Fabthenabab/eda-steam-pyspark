<img src="assets/Steam_Logo.png" alt="Steam Logo" width="300"/>

> **Exploratory data analysis of the Steam's videogames platform's Catalog Dataset.**  
> Analysis of the market on different levels: macro, genres, platform. The analysis is conducted with pyspark using Databricks platform.

---

## 📋 Table of Contents

- [📋 Table of Contents](#-table-of-contents)
- [🎯 About](#-about)
- [🎯 Project Goals](#-project-goals)
- [⚙️ Tech Stack](#️-tech-stack)
- [✨ Key Features](#-key-features)
  - [**Data Preparation \& Exploration**](#data-preparation--exploration)
  - [**Multi-Level Analysis**](#multi-level-analysis)
- [📊 Key Insights](#-key-insights)
- [📓 Notebooks](#-notebooks)
- [🚀 Quick Start](#-quick-start)
- [📜 License](#-license)
- [🎓 Portfolio Context](#-portfolio-context)

---

## 🎯 About

Steam is a video game digital distribution service and storefront from Valve.

As a game publisher, it's useful to better understand the videogames ecosystem and today's trends prior to launching a new game.

[⬆ Back to top](#-table-of-contents)

---

## 🎯 Project Goals

1. **Analysis at the "macro" level**: Biggest publisher, best rated games, most represented languages, ...
2. **Genres analysis**: Most represented genres, favorite genres among publishers, most lucrative games, ...
3. **Platform analysis**: Availability on different platforms (Linux,Mac, Windows), ...

[⬆ Back to top](#-table-of-contents)

---

## ⚙️ Tech Stack

![Databricks](https://img.shields.io/badge/Databricks-Runtime-FF3621?logo=databricks&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.8+-blue.svg?logo=python&logoColor=white)
![PySpark](https://img.shields.io/badge/PySpark-3.x-E25A1C?logo=apachespark&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-Spark_SQL-4479A1?logo=apachespark&logoColor=white)

[⬆ Back to top](#-table-of-contents)

---

## ✨ Key Features

### **Data Preparation & Exploration**
Comprehensive missing value analysis (null and empty strings), nested JSON structure handling (structs, arrays, multi-value strings). Data normalization through field explosion for genres, languages, and platforms.

### **Multi-Level Analysis**
- Macro-level: publisher rankings, release trends, price distribution, language coverage, age restrictions
- Genre-level: popularity, review sentiment, publisher specialization, price positioning
- Platform-level: availability distribution across Linux/Mac/Windows, genre-platform cross-analysis

[⬆ Back to top](#-table-of-contents)

---

## 📊 Key Insights

**Dataset:** 55,691 games from the Steam platform

1. **Fragmented publisher landscape** — the largest publisher (Big Fish Games) represents only 0.76% of all releases
2. **Steady growth in releases** with a notable dip in 2019 and a peak in 2021, possibly COVID-related
3. **Price distribution heavily skewed toward low-cost games**, with varying discount rates across price categories
4. **English dominates** language availability with a steep long tail
5. **Very few age restrictions** — only 0.55% of games are rated 16+ and 0.41% rated 18+
6. **Genre lucrativity ≠ genre popularity** — we lack sales volume data, so price positioning (avg price per genre) is used as a proxy rather than estimated revenue

[⬆ Back to top](#-table-of-contents)

---

## 📓 Notebooks

**[eda_steam.ipynb](notebooks/eda_steam.ipynb)** — Complete Exploratory Data Analysis
- Missing value handling (nulls and empty strings)
- Multi-value field explosion (genres, languages)
- Publisher and release trend analysis
- Price distribution and discount analysis
- Genre popularity, sentiment, and price positioning
- Cross-platform availability analysis

**[01_eda.html](https://fabthenabab.github.io/eda-steam-pyspark/01_eda.html)** — Full notebook export with Databricks visualizations

[⬆ Back to top](#-table-of-contents)

---

## 🚀 Quick Start

**Prerequisites:**
- Databricks workspace with cluster access
- Access to S3 dataset: `s3://full-stack-bigdata-datasets/Big_Data/Project_Steam/`

**Usage:**
```
# Import notebook into Databricks workspace

[⬆ Back to top](#-table-of-contents)

---

## 📜 License

This project is licensed under the GPL-3.0 License — see the [LICENSE](./LICENSE) file for details.

[⬆ Back to top](#-table-of-contents)

---

## 🎓 Portfolio Context

**Project Type:** Exploratory Data Analysis (EDA) — Big Data  
**Focus:** Distributed data exploration and insight discovery at scale

**Demonstrates:**
- **PySpark fluency** — DataFrame API and Spark SQL used interchangeably
- **Complex data wrangling** (nested JSON, multi-value field explosion, UDFs for normalization)
- **Analytical rigor** (proxy limitations acknowledged, statistical biases identified)
- **Big Data tooling** — Databricks, S3 data source, distributed computation
- **Business insight generation** from a 55k+ record dataset

📚 **Part of [Fab's Data Science Portfolio](https://github.com/fabthenabab)** — 
Several projects covering the full ML lifecycle from research to production.

[⬆ Back to top](#-table-of-contents)