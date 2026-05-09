# 🌿 Sustainable Brand Choice — Binary Logit Analysis
### EDA · Outlier Detection · Binary Logit Model | R · glm · ggplot2

> **Academic project** completed as part of the ANL553 Applied Statistical Methods
> and Causal Analysis module at Singapore University of Social Sciences (SUSS), 2025.
> Dataset: lifestyle and sustainability survey data (public/anonymised).

---

## 📌 Overview

This project explores **what predicts whether a consumer chooses sustainable brands**,
using lifestyle, behavioural, and demographic survey data from 499 respondents.

The analysis moves through three stages: thorough exploratory analysis,
outlier detection, and a binary logit model to identify the key drivers
of sustainable brand adoption.

---

## ❓ Research Question

> *Which lifestyle, behavioural, and demographic factors significantly predict
> a consumer's decision to choose sustainable brands?*

---

## 🔬 Methods

| Step | Method | Purpose |
|---|---|---|
| 1 | Descriptive statistics | Understand central tendency and spread |
| 2 | IQR outlier detection | Flag anomalies across numeric variables |
| 3 | Boxplot + Violin + Histogram | Visualise distributions and outliers |
| 4 | Frequency tables + bar charts | Explore categorical variable distributions |
| 5 | Binary Logit (`glm`, binomial) | Model probability of sustainable brand choice |
| 6 | Odds ratio interpretation | Quantify direction and magnitude of each predictor |
| 7 | Confusion matrix + hit rate | Evaluate model accuracy (76.2%) |

---

## 📊 Key Findings

### Significant Predictors (p < 0.05)

| Variable | Direction | Interpretation |
|---|---|---|
| **EnvironmentalAwareness** | ➕ Positive | Higher awareness → more likely to choose sustainable brands |
| **DietType (Animal-based)** | ➖ Negative | Animal-based diet significantly reduces probability |
| **EnergySource (Non-renewable)** | ➖ Negative | Non-renewable energy users avoid sustainable brands |
| **UsingPlasticProducts (Often)** | ➖ Negative | Frequent plastic users less likely to buy sustainable |
| **TransportationMode (Car)** | ➖ Negative | Car users show lower sustainable brand preference |

### Non-Significant Predictors
> **Age, Gender, Location** — sustainability choices cut across all demographic groups

### Model Performance
| Metric | Value |
|---|---|
| Overall Accuracy | **76.2%** |
| Sensitivity (True Positive) | **82.5%** |
| Specificity (True Negative) | **69.1%** |

---

## 💡 Business Implications

- **Target by lifestyle, not demographics** — diet, transport, and energy habits predict behaviour better than age or gender
- **Environmental awareness is the strongest lever** — education and awareness campaigns are more effective than demographic targeting
- **Segment into three clusters:**
  - *Eco-Conscious Actives* — plant-based, renewable energy, walking → promote innovation
  - *Balanced Pragmatists* — moderate awareness, mixed habits → emphasise easy swaps
  - *Traditional Consumers* — car users, plastic users → focus on cost and small habit shifts

---

## 🛠️ Tools & Packages

| Tool | Purpose |
|---|---|
| `R` | Core analysis language |
| `glm` (base R) | Binary logistic regression |
| `broom` | Tidy odds ratios and model outputs |
| `ggplot2` | All visualisations |
| `dplyr` + `tidyr` | Data wrangling and reshaping |
| `patchwork` | Side-by-side plot layouts |

---

## 🔗 Related Projects

- [📱 Mobile Game Downloads — Panel Data Analysis](https://github.com/thaotracy-sg/Causal-analysis-panel-logit-R-gameapp)
- [🔋 Electric Power & CO₂ Forecasting](https://github.com/thaotracy-sg/Time-series-forecasting-electric-power-co2-emission-europe)

---

*Analysis by Tracy Nguyen | ANL553 Applied Statistical Methods & Causal Analysis | SUSS 2025*
