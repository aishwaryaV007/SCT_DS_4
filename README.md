# 🚦 Traffic Accident Analysis — SkillCraft Technology Task 04

![Python](https://img.shields.io/badge/Python-3.x-blue) ![Pandas](https://img.shields.io/badge/Pandas-EDA-green) ![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-orange) ![Folium](https://img.shields.io/badge/Folium-Heatmap-red)

---

## 📌 Objective

Analyze US traffic accident data to identify patterns related to **road conditions**, **weather**, and **time of day**. Visualize accident hotspots and contributing factors using Python.

---

## 📂 Dataset

- **Source:** [US Accidents (2016–2023) — Kaggle](https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents)
- **Total Records:** ~7.7 million accident records across 49 US states
- **Records Used:** 500,000 (sampled for efficient analysis)
- **Features:** 46 columns including severity, location, weather, road conditions, and time

---

## 🛠️ Tools & Libraries

| Tool | Purpose |
|------|---------|
| Python 3.x | Core language |
| Pandas | Data loading, cleaning, feature extraction |
| Matplotlib | Static visualizations |
| Seaborn | Statistical plots |
| Folium | Interactive heatmap |

---

## 📁 Project Structure

```
task04_accident_analysis/
├── accident_analysis.ipynb       ← Main analysis notebook
├── accidents_by_hour.png         ← Accidents by hour of day
├── accidents_by_day.png          ← Accidents by day of week
├── accidents_by_month.png        ← Accidents by month
├── accidents_by_weather.png      ← Top weather conditions
├── severity_distribution.png     ← Severity levels chart
├── day_vs_night.png              ← Day vs Night comparison
├── road_features.png             ← Road features at accident sites
├── top_states.png                ← Top 10 states by accident count
├── correlation_heatmap.png       ← Weather factors vs Severity
├── accident_hotspot_map.html     ← Interactive geographic heatmap
└── README.md
```

---

## 🔍 Analysis Performed

### 1. Data Preprocessing
- Loaded only relevant 19 columns to optimize memory
- Parsed `Start_Time` to extract `Hour`, `Month`, `DayOfWeek`
- Dropped rows with null values in critical columns

### 2. Time-Based Analysis
- Accidents by **hour of day** — identifies rush hour peaks
- Accidents by **day of week** — identifies weekday vs weekend trends
- Accidents by **month** — identifies seasonal patterns

### 3. Weather Analysis
- Top 10 weather conditions during accidents
- Correlation between weather factors (visibility, humidity, wind speed, temperature) and severity

### 4. Road Condition Analysis
- Presence of road features (Junctions, Traffic Signals, Crossings, etc.) at accident sites

### 5. Geographic Analysis
- Top 10 states by accident count
- Interactive heatmap showing accident hotspots across the US

---

## 📊 Key Findings

- **Peak Hours:** Most accidents occur between **7–9 AM** and **4–6 PM** (rush hours)
- **Peak Day:** **Fridays** have the highest number of accidents
- **Seasonal Trend:** Accidents are higher in **winter months** (Oct–Dec)
- **Weather:** Most accidents occur in **Clear/Fair weather** due to higher traffic volume; however, **Fog and Snow** conditions lead to higher severity
- **Road Features:** **Traffic Signals** and **Junctions** are the most common road features at accident sites
- **Top States:** **California, Florida, and Texas** have the highest accident counts
- **Day vs Night:** Significantly more accidents occur **during the day**
- **Severity:** Majority of accidents fall under **Severity Level 2**

---

## ▶️ How to Run

```bash
# 1. Clone the repository
git clone https://github.com/your-username/task04-accident-analysis.git
cd task04-accident-analysis

# 2. Install dependencies
pip install pandas matplotlib seaborn folium

# 3. Download dataset from Kaggle and place it in the project folder
# Dataset: US_Accidents_March23.csv

# 4. Open and run the notebook
jupyter notebook accident_analysis.ipynb
```

---

## 📈 Sample Visualizations

> All charts are saved as `.png` files in the project folder.
> Open `accident_hotspot_map.html` in any browser to view the interactive heatmap.

---

## 👤 Author

**Aishwarya**  
Data Science Intern — SkillCraft Technology  
Task 04 | June 2026
