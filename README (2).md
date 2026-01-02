# Mobile Game Analytics: Player Behavior & Monetization Deep Dive

A comprehensive analytics case study examining player retention, monetization patterns, and behavioral segmentation in a mobile game with 26,000+ users and 15M+ events.

![Python](https://img.shields.io/badge/Python-3.10-blue)
![BigQuery](https://img.shields.io/badge/Google-BigQuery-orange)
![Status](https://img.shields.io/badge/Status-Complete-green)

---

## 📊 Overview

This project analyzes player behavior data from a mobile game to answer critical business questions:

1. **Retention**: How well does the game retain players at D1, D7, and D30?
2. **Monetization**: What drives payer conversion and LTV?
3. **Churn**: Where do players drop off, and why?
4. **Segmentation**: Can we identify distinct player archetypes for targeted strategies?

---

## 🔑 Key Findings

| Insight | Detail | Business Impact |
|---------|--------|-----------------|
| **Early Monetization Window** | 81% of first purchases occur at Level 1 | Optimize first-session offers |
| **Churn Hotspot** | Level 6 accounts for 23.5% of all churn | Investigate difficulty/content gap |
| **Grinder Opportunity** | High-engagement users with $0 spend | Target for conversion campaigns |
| **Revenue Concentration** | Top 10% of payers drive 60%+ of revenue | Whale retention is critical |

---

## 🛠️ Methodology

### Statistical Rigor
- **Windowed LTV** (LTV7, LTV30) to eliminate cohort age bias
- **Effect sizes + 95% CIs** alongside p-values
- **Bonferroni correction** for multiple comparisons
- **Non-parametric tests** (Mann-Whitney U, Kruskal-Wallis) for skewed distributions

### Player Segmentation
Rule-based segmentation (not clustering) for interpretability and actionability:

| Archetype | Definition |
|-----------|------------|
| **Whale** | Top 1% of spenders |
| **Grinder** | $0 spend + top 10% engagement |
| **Casual** | Moderate engagement |
| **Newbie** | Never reached Level 2 |

---

## 📈 Visualizations

The notebook includes:
- Retention curves by cohort
- Windowed LTV comparison (bias-corrected)
- Churn vs. First Purchase by level
- Player archetype radar chart
- Revenue concentration analysis

---

## 🗂️ Repository Structure

```
├── mobile_game_analytics_final.ipynb   # Main analysis notebook
├── README.md                           # This file
```

---

## ⚙️ Tech Stack

- **Database**: Google BigQuery
- **Language**: Python 
- **Libraries**: pandas, numpy, scipy, matplotlib, seaborn
- **Environment**: Google Bigquery (Include Colab's jupyter notebook within BigQuery)


---

## 📝 Key Analytical Techniques Demonstrated

- Cohort analysis with proper observation windows
- Statistical hypothesis testing with effect sizes
- Bootstrap confidence intervals
- Multiple comparison corrections
- Feature engineering for player profiling
- Business-oriented segmentation

