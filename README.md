# Commercial Building Energy Performance Benchmarking (Singapore)

This project analyzes the energy performance of commercial buildings in Singapore using publicly available data. The focus is on understanding patterns in **Energy Use Intensity (EUI)** across building functions, size categories, and HVAC plant efficiency, as well as how energy performance has changed over time.

The goal of this analysis is to support informed decision-making in **sustainable building operations**, **energy management**, and **retrofit planning**.

---

## Dataset

**Source:** Singapore Open Data Portal (Data.gov.sg)  
**Years Covered:** 2017–2020  
**Scope:** Commercial buildings with reported annual Energy Use Intensity (kWh/m²·yr)

Key variables used in this project:
- Main building function (e.g., Office, Retail, Hotel)
- Gross floor area
- Building size category (Small / Large)
- Centralized air-conditioning plant efficiency (kW/RT)
- Annual EUI (kWh/m²·yr)

---

## Tools and Libraries

| Purpose | Tools |
|--------|------|
| Data Cleaning & Analysis | Python (Pandas, NumPy) |
| Visualization | Matplotlib, Seaborn |
| Notebook Execution | Jupyter Notebook |

---

## Key Visualizations & Insights

### 1) Distribution of EUI (2020) for Commercial Buildings
The distribution shows **wide variation** in EUI across commercial buildings.  
Some buildings exhibit **very high EUI**, indicating operational intensity or potential inefficiencies.

**Median EUI (2020): ~190 kWh/m²·yr**

---

### 2) EUI (2020) by Main Building Function
Hotels consistently show **higher EUI**, likely due to continuous occupancy and hospitality amenities.  
Retail and Office buildings show **lower and more stable** energy intensity patterns.

| Function | Approx. Median EUI | Interpretation |
|---------|--------------------|----------------|
| Retail | Lowest | More consistent operational patterns |
| Office | Moderate | Efficiency depends on occupancy and controls |
| Mixed Dev. | Higher variability | Diverse usage mix |
| Hotel | Highest | 24/7 operation & cooling requirements |

---

### 3) EUI (2020) by Building Size Category
Larger buildings tend to operate **more efficiently per square meter**, benefiting from economies of scale and more standardized facility management.

| Size Category | Median EUI (approx.) | Comment |
|--------------|----------------------|---------|
| Large | ~187 | More stable, efficient |
| Small | ~224 | Higher variation, less scale advantage |

---

### 4) AC Plant Efficiency vs EUI (2020)
The correlation between centralized AC plant efficiency and EUI is **weak** *(r ≈ -0.05)*.

This suggests that:
- **Operational control strategies**
- **Occupancy schedules**
- **Building usage patterns**

have a more significant impact on EUI than equipment efficiency ratings alone.

---

### 5) Trend in Mean EUI (2017 → 2020)
Mean EUI declines gradually from 2017 to 2019, followed by a **sharp reduction in 2020**.

This 2020 decrease aligns with:
- **Reduced building occupancy** during COVID-19, rather than efficiency upgrades alone.

---

## Conclusion

This benchmarking analysis reveals meaningful differences in commercial building energy performance:

- **Building function** significantly influences EUI, with hotels being the highest consumers.
- **Larger buildings typically operate more efficiently** at scale.
- **Equipment efficiency alone does not determine actual energy performance**—operations matter.
- Trends in annual EUI must be interpreted in context (e.g., pandemic-related occupancy changes).

Understanding these patterns can guide **energy optimization strategies**, **retrofit targeting**, and **sustainable building management**.

---

## Repository Structure (Recommended)
project/
│ README.md
│ requirements.txt
│
├── data/
│ raw_data.csv
│ cleaned_data.csv
│
├── notebooks/
│ analysis.ipynb
│
└── visuals/
v1_eui_distribution.png
v2_eui_by_function.png
v3_eui_by_size.png
v4_ac_efficiency_vs_eui.png
v5_eui_trend.png


