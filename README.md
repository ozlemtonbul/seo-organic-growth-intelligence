# Vicco SEO Organic Growth Intelligence Pipeline

This repository contains a production-grade machine learning and decision intelligence engine designed to optimize organic SEO growth.

## What the System Does
It converts historical page-level SEO data (clicks, impressions, position, CTR) into an actionable decision-support system. It goes beyond simple reporting by providing predictive insights, simulating optimization scenarios, and recommending specific SEO actions based on cost, effort, and projected Return on Investment (ROI).

## Problem It Solves
Traditional SEO reporting tools provide backward-looking metrics (what happened) but fail to provide prescriptive guidance (what to do next). They do not account for the effort or cost required to implement an SEO change, nor do they simulate the expected business value of that change. This system solves that limitation by acting as a predictive and prescriptive engine.

## System Architecture
The pipeline follows a robust, end-to-end architecture:
1. **Data Ingestion & KPI Engineering**: Processes raw SEO data and computes derived metrics like traffic value, visibility score, and rank strength.
2. **Feature Engineering**: Generates time-based, lag-based, and trend signals for machine learning models.
3. **Predictive Modeling**: Utilizes Random Forest Regressors to predict next-period clicks and impressions.
4. **Scenario Simulation Engine**: Simulates the impact of different SEO actions (Maintain, Title/Meta Optimization, Content Refresh, Internal Linking Improvement).
5. **Business Value Layer**: Evaluates each scenario against expected costs to compute incremental traffic value, net value, and ROI.
6. **Recommendation & Guardrails**: Recommends the highest ROI action. If the model's predictive confidence is low, aggressive recommendations are downgraded to "Review".
7. **Prioritization Engine**: Classifies pages into High, Medium, or Low priority based on net value and ROI.

## Core Capabilities
- **Predictive SEO Modeling**: Machine learning models predicting future clicks and impressions based on historical performance.
- **Scenario Simulation**: 'What-if' analysis for different SEO interventions.
- **ROI-Based Prioritization**: Ranking SEO tasks by their expected return on investment.
- **Cost-Effort Modeling**: Evaluating the required resources against projected gains.
- **Recommendation Engine**: Actionable, page-level guidance.

## Business Value
- **Better SEO Prioritization**: Focus resources on pages with the highest upside.
- **Improved Organic ROI**: Maximize the impact of your SEO budget and time.
- **Reduced Wasted Effort**: Avoid optimizing pages that offer minimal incremental value.
- **Data-Driven Strategy**: Move from gut-feeling SEO to quantitative decision intelligence.

## Outputs
For every page in the dataset, the system outputs:
- Action recommendations (e.g., Optimize, Improve Content, Internal Linking, Maintain, Review).
- ROI and net value analysis.
- Scenario comparisons (predicted uplift vs. baseline).
- High/Medium/Low priority tagging.

## How to Run

1. Clone the repository and navigate to the project root.
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Set up your configuration file:
   ```bash
   cp .env.example .env
   ```
   *Edit `.env` to ensure your data paths and cost parameters are correct.*
4. Run the intelligence pipeline:
   ```bash
   python src/seo_organic_growth_intelligence.py
   ```

## Author
Ozlem Tonbul
