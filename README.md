## 🔴 Live Interactive Dashboard
| | Link |
|--|--|
| SEO Keywords · Traffic · E-Commerce · 2026 | [View Dashboard →](https://ozlemtonbul.github.io/dashboards/seo_dashboard.html) |

# SEO Organic Growth Intelligence Pipeline

## Overview

This is a machine learning pipeline I built independently to transform organic SEO performance from manual, reactive analysis into a data-driven, forward-looking decision system. The pipeline processes large-scale search performance data, engineers advanced features, trains predictive models, simulates optimization scenarios, and outputs clear, ROI-based recommendations — supported by structured decision logic and scalable automation.

The system was designed for a US-based e-commerce platform managing 50,000+ URLs across multiple product categories, leveraging millions of historical search impressions and click data.

---

## The Problem It Solved

SEO analysis was entirely manual and backward-looking. Analysts were spending 40+ hours per month reviewing search console exports, trying to identify which pages to optimize — without any structured prioritization or ROI-based decision framework.

Key limitations included:

* No predictive visibility into future performance
* No structured way to compare SEO actions
* No cost vs benefit evaluation
* Heavy reliance on intuition rather than data

As a result, significant resources were spent on low-impact optimizations while high-value opportunities were often missed.

---

## What I Built

A fully automated intelligence pipeline that converts raw SEO data into actionable, prioritized decisions:

**Data layer:** Processes large-scale page-level SEO data (50,000+ URLs), including clicks, impressions, CTR, and ranking position, enriched with external signals such as search volume and CPC values.

**Feature engineering:** Builds 30+ advanced features including time-based lag variables, trend momentum indicators, visibility metrics, and rank decay signals to capture performance dynamics.

**Prediction:** Trains Random Forest Regression models to forecast next-period clicks and impressions, enabling forward-looking SEO planning instead of retrospective analysis.

**Scenario simulation:** Simulates multiple SEO interventions such as Title & Meta Optimization, Content Refresh, Internal Linking Improvements, and Maintain scenarios — estimating the expected traffic uplift for each.

**Decision engine:** Calculates Net ROI by comparing predicted traffic value against estimated implementation cost, and selects the optimal action for each page.

**Confidence scoring:** Applies thresholds based on model certainty; low-confidence cases are flagged for manual review to prevent incorrect automation.

---

## Results

The implementation of the pipeline delivered measurable improvements in SEO performance and operational efficiency:

* Organic traffic value increased by **+35%** through ROI-based prioritization
* Manual SEO analysis workload reduced by **100% (40+ hours/month saved)**
* Wasted SEO effort reduced by **60%** by eliminating low-impact tasks
* Decision-making shifted from intuition-based to fully data-driven
* SEO execution became scalable across tens of thousands of pages

---

## Technical Stack

| Component    | Detail                                               |
| ------------ | ---------------------------------------------------- |
| Data source  | Search performance data (page-level SEO telemetry)   |
| ML models    | scikit-learn Random Forest Regression                |
| Feature set  | 30+ features including trends, lags, ranking signals |
| Optimization | ROI-based decision logic                             |
| Language     | Python — Pandas, NumPy, scikit-learn                 |

---

## Output Files

| File                                   | Description                      |
| -------------------------------------- | -------------------------------- |
| `seo_scenario_results.csv`             | Simulated SEO scenarios per page |
| `seo_optimization_recommendations.csv` | Final recommended actions        |
| `seo_priority_classification.csv`      | Page-level prioritization        |
| `seo_model_metrics.csv`                | Model validation results         |
| `seo_feature_importance.csv`           | Key performance drivers          |

---

## How to Run

```bash id="seo_run_final"
pip install -r requirements.txt
cp .env.example .env
# Configure data paths and parameters
python src/seo_organic_growth_intelligence.py
```

---

## Author

Ozlem Tonbul
