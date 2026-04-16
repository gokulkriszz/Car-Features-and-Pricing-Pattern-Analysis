<div align="center">

<img src="https://images.unsplash.com/photo-1492144534655-ae79c964c9d7?w=900&auto=format&fit=crop&q=80" width="100%" height="200px" style="object-fit:cover; border-radius:12px;" alt="Car Banner"/>

# 🚗 Car Features & Pricing Pattern Analysis

**What makes a car expensive? Data has the answer.**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Google Colab](https://img.shields.io/badge/Google_Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-28a745?style=for-the-badge)

</div>

---

## 📌 Project Overview

The global automobile industry is driven by a complex mix of performance specs, fuel technology, and brand positioning. This project performs a **full-stack data analysis** on 2025 car models — from raw data cleaning all the way to an interactive Power BI dashboard.

> _"Every feature on a car has a price tag. This project quantifies exactly that."_

The analysis explores how **engine capacity, horsepower, fuel type, and brand** influence car pricing and market adoption trends across global manufacturers.

---

## 🎯 Objectives

- 🔍 Identify the **key features that drive car prices** up or down
- 🏎️ Compare **brand-wise pricing and performance** trends
- ⚡ Analyze **EV (Electric Vehicle) adoption** vs traditional fuel types
- 🌍 Uncover **global market patterns** across manufacturers
- 📊 Visualize findings in an **interactive Power BI dashboard**

---

## 🛠️ Tools & Libraries

| Tool / Library | Purpose |
|----------------|---------|
| 🐍 Python | Core programming language |
| ☁️ Google Colab | Cloud-based notebook environment |
| 🐼 Pandas | Data manipulation & cleaning |
| 🔢 NumPy | Numerical computations |
| 📊 Matplotlib | Static visualizations |
| 🎨 Seaborn | Statistical data visualization |
| 📈 Power BI | Interactive dashboard (`.pbit`) |

---

## 📂 Repository Structure

```
Car-Features-and-Pricing-Pattern-Analysis/
│
├── 📓 Cars_Dataset_(2025)_DA_FP.ipynb       # Main analysis notebook (Colab)
├── 📄 Cars Datasets 2025.csv                # Raw dataset
├── 📄 car_dataset_2025_cleaned.csv          # Cleaned dataset
├── 📊 car_dataset_2025.pbit                 # Power BI dashboard template
└── 📄 README.md                             # Project documentation
```

---

## 🔄 Project Workflow

```
Raw Data  ──►  Data Cleaning  ──►  EDA  ──►  Visualizations  ──►  Power BI Dashboard
   📄                🧹              🔍            📈                    📊
```

### Step 1 — 🧹 Data Cleaning & Preprocessing
- Handled missing values across price, engine, and performance columns
- Standardized fuel type categories and brand names
- Removed outliers and duplicate records
- Exported cleaned data to `car_dataset_2025_cleaned.csv`

### Step 2 — 🔍 Exploratory Data Analysis (EDA)
- **Univariate** — distribution of price, horsepower, engine size
- **Bivariate** — price vs horsepower, fuel type vs price
- **Multivariate** — brand × fuel type × price heatmaps and pair plots

### Step 3 — 📊 Power BI Dashboard
- Interactive filters by brand, fuel type, and price range
- Visual comparison of EV vs ICE vehicle pricing
- Top brands by average horsepower and price

---

## 📈 Key Insights

- 🏆 **Engine capacity** is the strongest predictor of car price across all brands
- ⚡ **Electric vehicles** are priced significantly higher on average than petrol/diesel counterparts
- 🌟 **Luxury brands** (BMW, Mercedes, Audi) cluster in high horsepower + high price quadrant
- 📉 **Fuel efficiency** shows a negative correlation with horsepower in ICE vehicles
- 🚘 **SUVs and crossovers** dominate the mid-to-premium price segment in 2025

---

## 💡 Sample Analysis Code

```python
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

df = pd.read_csv('car_dataset_2025_cleaned.csv')

# Price distribution by fuel type
plt.figure(figsize=(10, 6))
sns.boxplot(data=df, x='Fuel_Type', y='Price', palette='Set2')
plt.title('Car Price Distribution by Fuel Type (2025)', fontsize=14)
plt.xlabel('Fuel Type')
plt.ylabel('Price (USD)')
plt.tight_layout()
plt.show()
```

---

## 🚀 How to Run

### ☁️ Option 1 — Run in Google Colab (Recommended)

1. Click the **Open in Colab** badge below:

   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/gokulkriszz/Car-Features-and-Pricing-Pattern-Analysis/blob/main/Cars_Dataset_(2025)_DA_FP.ipynb)

2. Upload the dataset when prompted:
```python
   from google.colab import files
   uploaded = files.upload()  # Upload Cars Datasets 2025.csv
```

3. Run all cells top to bottom — **no installation needed!**

---

### 💻 Option 2 — Run Locally

1. **Clone the repository**
```bash
   git clone https://github.com/gokulkriszz/Car-Features-and-Pricing-Pattern-Analysis.git
   cd Car-Features-and-Pricing-Pattern-Analysis
```

2. **Install dependencies**
```bash
   pip install pandas numpy matplotlib seaborn jupyter
```

3. **Launch Jupyter Notebook**
```bash
   jupyter notebook Cars_Dataset_\(2025\)_DA_FP.ipynb
```

---

### 📊 Option 3 — View Power BI Dashboard

Open `car_dataset_2025.pbit` in [Power BI Desktop](https://powerbi.microsoft.com/desktop/) and connect it to `car_dataset_2025_cleaned.csv`.

---

## 📸 Dashboard Preview

> _Add a screenshot of your Power BI dashboard here!_
> `![Dashboard Preview](your-screenshot-link.png)`

---

## 🙋‍♂️ Author

<div align="center">

**Gokul Krishnan**

[![GitHub](https://img.shields.io/badge/GitHub-gokulkriszz-181717?style=for-the-badge&logo=github)](https://github.com/gokulkriszz)

_"From raw specs to real insights — data drives every decision."_

</div>
