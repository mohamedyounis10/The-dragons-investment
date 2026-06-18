<div align="center">
  <h1>China's Global Investment Analysis 🇨🇳🌍📊</h1>
  <p>End-to-end analysis of China's worldwide funding & development projects (EDA 🔍 → preprocessing 🧹 → visualization 📈) using Python and Power BI 🚀.</p>

  <p>
    <a href="#overview">Overview 🧾</a> •
    <a href="#project-structure">Project Structure 🗂️</a> •
    <a href="#dataset">Dataset 🧩</a> •
    <a href="#results">Results 📊</a> •
    <a href="#dashboard">Dashboard 🖥️</a>
  </p>

  <p>
    <img alt="Python" src="https://img.shields.io/badge/Python-3.x-blue" />
    <img alt="Jupyter" src="https://img.shields.io/badge/Jupyter-Notebook-orange" />
    <img alt="Pandas" src="https://img.shields.io/badge/Pandas-Data_Analysis-150458" />
    <img alt="Matplotlib" src="https://img.shields.io/badge/Matplotlib-Visualization-blue" />
    <img alt="Seaborn" src="https://img.shields.io/badge/Seaborn-Visualization-4C72B0" />
    <img alt="PowerBI" src="https://img.shields.io/badge/PowerBI-Dashboard-F2C811" />
  </p>
</div>

---

## Table of Contents 🧭

- [Overview 🧾](#overview)
- [Project Structure 🗂️](#project-structure)
- [Dataset 🧩](#dataset)
- [Results 📊](#results)
- [Dashboard 🖥️](#dashboard)
- [How to Run ▶️](#how-to-run)
- [Author ✍️](#author-️)

---

<a id="overview"></a>
## Overview 🧾

This repository focuses on **China's Global Investment & Funding Analysis**, exploring how China allocates financial and development resources across the world through:

- **Data Cleaning 🧹**: Selecting key project columns, handling missing values, and removing duplicate entries.
- **EDA 🔍**: Analyzing funding flows across regions, recipient countries, sectors, and commitment years.
- **Key Metrics 📈**: Calculating total project funding, project volume, regional distribution, and average project duration.
- **Visualization 🎨**: Using `Matplotlib` and `Seaborn` for geographic, sectoral, and temporal data storytelling.

---

<a id="project-structure"></a>
## Project Structure 🗂️

- [`Dataset/` 🧩](#dataset) — China's global funding & project records
  - `ChineseFinancialPublicDiplomacyProjectDetails.xlsx`
- [`Dashboard/` 🖥️](#dashboard) — interactive reports
  - `China.pbix` (Power BI Report)
- [`notebook.ipynb` 📒](#notebook) — full analysis workflow

Tree 🌳:

```text
China Analysis/
├─ Dashboard/
│  └─ China.pbix
├─ Dataset/
│  └─ ChineseFinancialPublicDiplomacyProjectDetails.xlsx
└─ notebook.ipynb
```

---

<a id="dataset"></a>
## Dataset 🧩

The analysis is performed on the **Chinese Financial & Public Diplomacy Project Details** dataset (AidData), containing **69 columns** and **10,741 rows** of project-level records spanning commitments from **2000 to 2017**.

Target Columns 🎯:
- **`amount_nominal`**: Project funding amount in original currency.
- **`amount_constant_usd2017`**: Inflation-adjusted funding in constant 2017 USD.

Key Features 🧾:
- `project_id`, `status`, `type`, `donor`, `recipient`, `recipient_region`.
- `sector_name`, `flow_type`, `commitment_year`.
- `implementation_start_year`, `completion_year`.

---

<a id="results"></a>
## Results 📊

### Key Performance Indicators (KPIs) 🧪

From the notebook analysis 🖨️:

| Metric | Value |
|---|---:|
| **Total Projects** | **10,741** |
| **Total Funding** | **$746.05 Billion** |
| **Average Project Duration** | **1.27 years** |
| **Regions Covered** | **6** (Africa, America, Asia, Europe, Middle East, Oceania) |

### Top Recipients by Region 💡

| Region | Top Recipient | Total Funding (USD) |
|---|---|---:|
| **Africa** | Angola | $52.7 B |
| **America** | Venezuela | $91.1 B |
| **Asia** | Kazakhstan | $42.3 B |
| **Europe** | Russia | $125.4 B |
| **Middle East** | Iran | $17.1 B |
| **Oceania** | Papua New Guinea | $6.1 B |

### Insights 💡
- **Global Reach**: China's funding projects span all major world regions, with strong concentration in Africa, Asia, and Latin America.
- **Sector Diversity**: Analysis covers top sectors including transport, energy, and communications infrastructure.
- **Temporal Trend**: Commitment volumes show evolving patterns across years, reflecting shifts in China's overseas development strategy.
- **Funding Types**: Projects include loans, grants, and mixed financial flows across public diplomacy and development finance.

---

<a id="dashboard"></a>
## Dashboard 🖥️

An interactive **Power BI Dashboard** is included to provide a visual breakdown of:
- Funding by recipient country & region.
- Project status and sector distribution.
- Trends over commitment years.
- Top sectors and funding flow types.

Check [`Dashboard/China.pbix`](Dashboard/China.pbix) to explore the interactive report.

![China Investment Dashboard](Dashboard/China%20Intro.jpg)

---

<a id="how-to-run"></a>
## How to Run ▶️

### 1) Setup Environment 🧪
```bash
python -m venv .venv
.\.venv\Scripts\activate
```

### 2) Install Dependencies 📦
```bash
pip install pandas numpy matplotlib seaborn jupyter openpyxl
```

### 3) Launch Notebook 🚀
```bash
jupyter notebook
```
Open `notebook.ipynb` 📒 to see the full analysis.

---

## Author ✍️

- **Name**: Mohammed Younis

---
