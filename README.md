<div align="center">

<img src="https://img.shields.io/badge/-%F0%9F%9B%92%20BLINKIT%20GROCERY%20ANALYSIS-F9C923?style=for-the-badge&logoColor=black" height="42"/>

<br/><br/>

<img src="https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black"/>
<img src="https://img.shields.io/badge/DAX-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white"/>
<img src="https://img.shields.io/badge/Power%20Query-217346?style=for-the-badge&logo=microsoft&logoColor=white"/>
<img src="https://img.shields.io/badge/Status-Complete-2A7E4C?style=for-the-badge"/>
<img src="https://img.shields.io/badge/License-MIT-F9C923?style=for-the-badge"/>

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=F9C923&height=120&section=header&text=Blinkit%20Sales%20Dashboard&fontSize=32&fontColor=0F1923&fontAlignY=65&animation=fadeIn"/>

### 🛒 An interactive Power BI dashboard analysing Blinkit's grocery sales
### across outlets, product categories and customer ratings

<br/>

[![⭐ Star this repo](https://img.shields.io/badge/⭐_Star_this_repo-F9C923?style=for-the-badge&logoColor=black)](.)
[![🍴 Fork](https://img.shields.io/badge/🍴_Fork-0F1923?style=for-the-badge&logoColor=white)](.)

</div>

<br/>

---

## 📌 Table of Contents

| # | Section |
|---|---------|
| 01 | [📊 Key Metrics — KPIs](#-key-metrics--kpis) |
| 02 | [🎨 Charts & Visuals](#-charts--visuals) |
| 03 | [🎛️ Interactive Slicers](#️-interactive-slicers) |
| 04 | [🗂️ Dataset & Fields](#️-dataset--fields) |
| 05 | [🚀 Getting Started](#-getting-started) |
| 06 | [💡 Key Insights](#-key-insights) |
| 07 | [🛠️ Tech Stack](#️-tech-stack) |
| 08 | [👤 Author](#-author) |

---

## 🖼️ Dashboard Preview

<div align="center">

> 📸 *Add your dashboard screenshot below*

<!-- Replace with your actual screenshot -->
<img src="assets/dashboard-preview.png" width="90%" alt="Blinkit Dashboard Preview" />

</div>

---

## 📊 Key Metrics — KPIs

<div align="center">

| 💰 Total Sales | 📈 Avg Sales | 📦 No. of Items | ⭐ Avg Rating |
|:-:|:-:|:-:|:-:|
| Aggregate revenue across all outlets | Mean sales value per outlet | Total distinct SKUs tracked | Avg customer satisfaction score |

</div>

> These four KPI cards sit at the **top of the dashboard** and update dynamically based on all active slicer selections.

---

## 🎨 Charts & Visuals

<div align="center">

| # | 📊 Visual Type | 💬 What It Shows |
|:-:|----------------|------------------|
| 1 | 🍩 **Donut Chart** | Sales split by **Item Fat Content** — Low Fat vs Regular |
| 2 | 🍩 **Donut Chart** | Revenue contribution by **Outlet Size** — Small / Medium / Large |
| 3 | 📊 **Bar Chart** | Total Sales broken down by **Item Type** — 16+ grocery categories |
| 4 | 📊 **Clustered Bar Chart** | Fat Content performance across **Outlet Location Tiers** 1 / 2 / 3 |
| 5 | 📉 **Line Chart** | Sales trend tracked by **Outlet Establishment Year** |
| 6 | 🔻 **Funnel Chart** | Sales funnel across **Outlet Location Types** |
| 7 | 🧮 **Matrix Table** | Outlet Type × Sales, Avg Sales, Items, Rating, Visibility |
| 8 | 🖼️ **KPI Image Cards** | Custom-branded icon cards for each headline metric |

</div>

---

## 🎛️ Interactive Slicers

> Slice the **entire dashboard dynamically** — every visual responds instantly.

<div align="center">

| 🏷️ Item Type | 📍 Outlet Location Type | 🏪 Outlet Size | 📐 Metrics Selector |
|:-:|:-:|:-:|:-:|
| Filter by grocery category | Tier 1 / Tier 2 / Tier 3 | Small / Medium / Large | Switch metric focus |

</div>

---

## 🗂️ Dataset & Fields

<details>
<summary><b>📋 Click to expand — Data Columns</b></summary>

<br/>

```
🏷️  Item Type                   —  Category of grocery item
🥗  Item Fat Content             —  Low Fat or Regular
🏪  Outlet Type                  —  Supermarket / Grocery Store
📐  Outlet Size                  —  Small, Medium, or High
📍  Outlet Location Type         —  Tier 1, Tier 2, or Tier 3 city
📅  Outlet Establishment Year    —  Year the outlet was established
💰  Sales                        —  Revenue from item sold
👁️  Item Visibility              —  Shelf visibility score (0–1)
⭐  Rating                       —  Customer satisfaction score
```

</details>

<details>
<summary><b>🧮 Click to expand — DAX Measures</b></summary>

<br/>

```dax
-- Total revenue across all outlets and item types
Total Sales = SUM('BlinkIT Grocery Data'[Sales])

-- Mean sales value per transaction / outlet
Avg Sales = AVERAGE('BlinkIT Grocery Data'[Sales])

-- Count of distinct items in the dataset
No of Items = COUNTROWS('BlinkIT Grocery Data')

-- Average customer satisfaction rating
Avg Rating = AVERAGE('BlinkIT Grocery Data'[Rating])
```

</details>

---

## 🚀 Getting Started

**Prerequisites:** [Power BI Desktop](https://powerbi.microsoft.com/desktop/) — free download

```bash
# Step 1 — Clone this repository
git clone https://github.com/your-username/blinkit-analysis.git

# Step 2 — Open the project folder
cd blinkit-analysis
```

**Step 3** → Open `Blinkit_Analysis.pbix` in Power BI Desktop

**Step 4** → Data model is fully embedded — ✅ no external source setup needed

**Step 5** → Use the slicers on the left panel to explore the data

> 💡 **Tip:** Use the **Metrics Selector** slicer to switch the KPI focus across all visuals simultaneously.

---

## 💡 Key Insights

<div align="center">

| Insight | Finding |
|---------|---------|
| 🥗 **Fat Content** | Low Fat items lead total sales — reflecting a health-conscious consumer shift |
| 🏙️ **Location Tiers** | Tier 3 outlets generate surprisingly competitive revenue vs urban locations |
| 📅 **Outlet Age** | Newer outlets consistently outperform older ones in the line chart trend |
| 🛒 **Outlet Type** | Supermarket Type 1 dominates both volume and item visibility in the matrix |
| ⭐ **Ratings** | Scores stay consistent across all outlet types — uniform service quality chain-wide |

</div>

---

## 🛠️ Tech Stack

<div align="center">

<img src="https://img.shields.io/badge/Power%20BI%20Desktop-F2C811?style=flat-square&logo=powerbi&logoColor=black"/>
<img src="https://img.shields.io/badge/DAX%20Measures-0078D4?style=flat-square&logo=microsoftazure&logoColor=white"/>
<img src="https://img.shields.io/badge/Power%20Query%20(M)-217346?style=flat-square&logo=microsoft&logoColor=white"/>
<img src="https://img.shields.io/badge/Data%20Modelling-E05C2D?style=flat-square"/>
<img src="https://img.shields.io/badge/Custom%20Theme-F9C923?style=flat-square&logoColor=black"/>

<br/><br/>

| Tool | Purpose |
|------|---------|
| **Power BI Desktop** | Report authoring, visuals, data modelling, publishing |
| **DAX** | Custom measures — Total Sales, Avg Sales, Avg Rating, Item Count |
| **Power Query (M)** | Data transformation, cleansing, column typing |
| **Custom Theme** | Branded colour palette aligned with Blinkit's identity |
| **Static Resources** | Custom KPI icon images embedded in the report |

</div>

---

## 👤 Author

<div align="center">

<img src="https://img.shields.io/badge/Your%20Name-Data%20Analyst-F9C923?style=for-the-badge&logo=powerbi&logoColor=black"/>

<br/><br/>

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ANALYST-AHTESHAM)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/your-profile)
[![Portfolio](https://img.shields.io/badge/Portfolio-F9C923?style=for-the-badge&logo=vercel&logoColor=black)](https://your-portfolio.com)

<br/>

**⭐ If this project helped you, please give it a star — it helps others find it! ⭐**

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=F9C923&height=100&section=footer&fontColor=0F1923&animation=fadeIn"/>

**Made with 💛 and Power BI**

*© 2026 Your Name · MIT License*

</div>
