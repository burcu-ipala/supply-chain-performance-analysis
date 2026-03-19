# D2C Marketplace Performance: How Operational Decisions Drive Customer Outcomes

## Business Context
Delivery performance is a critical operational KPI for any D2C e-commerce business. Late deliveries increase customer churn, damage brand reputation, and signal underlying inefficiencies in supplier and logistics processes. This project analyzes 100,000+ real orders from a Brazilian e-commerce platform to identify the root causes of delivery delays, segment sellers by operational performance, and quantify the relationship between supply chain KPIs and customer satisfaction.

## Research Questions
1. What operational factors most strongly predict delivery delays — and which product or seller segments carry the highest risk?
2. Can we identify distinct seller performance clusters that indicate where process interventions would have the most impact?
3. How does delivery performance affect customer satisfaction scores, and does this vary by product category or region?

## Key Findings
1. **Late delivery is the single biggest driver of dissatisfaction** — late orders average 2.26 review score vs 4.21 for on-time orders (-1.95 points). Regression confirms `is_late` as the strongest predictor (coef = -1.77).

2. **Processing time is the critical operational lever** — orders processed in 0–1 days have a 4.7% late rate; beyond 5 days it doubles to 11%; beyond 10 days it reaches 30.3%. A 3-day processing SLA would materially improve platform performance.

3. **25% of sellers generate disproportionate dissatisfaction** — K-Means clustering identified a High Risk segment (306 sellers) with a 13% late rate and 3.72 avg review, vs High Performers (876 sellers) at 4% late and 4.27 avg review. Targeted SLA enforcement on this segment is the highest-impact intervention.

4. **Price does not drive satisfaction — operations do** — price correlation with review score is 0.003 (negligible). D2C brands should invest in operational excellence over pricing strategy to improve customer retention.

## Dataset
[Olist Brazilian E-Commerce Dataset](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)  
100,000+ orders · 9 relational tables · 2016–2018

## Methods
- Data cleaning & feature engineering (Pandas)
- Exploratory data analysis & KPI visualization (Seaborn, Matplotlib)
- Linear & logistic regression — satisfaction and delay prediction (Statsmodels)
- K-Means clustering — seller performance segmentation (scikit-learn)

## Tools
Python · Pandas · Statsmodels · scikit-learn · Seaborn · Matplotlib

## How to Run
1. Download the dataset from Kaggle (link above) and place CSV files in the `data/` folder
2. Install dependencies: `pip install -r requirements.txt`
3. Run notebooks in order: 01 → 02 → 03 → 04 → 05

## Project Status
✅ Complete
