# ABG Motors: India Market Entry Feasibility Analysis

## 📊 Executive Summary
This project evaluates the feasibility of ABG Motors' expansion into the Indian market. By leveraging historical sales data and applying logistic regression forecasting to a dataset of **70,000 potential leads**, this analysis determines if the market can meet the minimum threshold of **12,000 units**.

**Final Verdict: PROCEED**
* **Target Requirement:** 12,000 units
* **Predicted Demand:** 15,848 units
* **Conversion Efficiency:** 22.6%

## 🛠️ Tech Stack
* **Python:** Data Cleaning, Feature Engineering (Z-Score Normalization), and Logistic Regression Forecasting.
* **Pandas/Seaborn:** Statistical distribution analysis.
* **Tableau:** Executive Dashboarding and Lifecycle Analysis.

## 📂 Project Structure

## 📂 Project Structure

* **[01_data](./01_data/)**
    * **[01_raw](./01_data/01_raw/)** — Unprocessed Japanese & Indian datasets.
    * **[02_processed](./01_data/02_processed/)** — Cleaned Japanese & Indian datasets.
    * **[03_forecasted_results](./01_data/03_forecast_results/)** — Final prediction output (15,848 leads).
* **[02_notebooks](./02_notebooks/)**
    * `01_data_preprocessing_and_eda.ipynb` — Data cleaning and exploration.
    * `02_classification_modeling.ipynb` — Logistic Regression training.
    * `03_indian_market_forecast.ipynb` — Z-Score alignment and 0.75 threshold.
* **[03_models](./03_models/)**
    * `abg_log_reg_model.pkl` — Serialized model.
    * `abg_scaler.pkl` — Saved Z-score scaler.
* **[04_visuals](./04_visuals/)** — Tableau Dashboard & Python trend plots.


01_raw/ — Unprocessed Japanese & Indian datasets.

02_processed/ — Cleaned Japanese & Indian datasets.

03_forecasted_results/ — Final prediction output (15,848 high-intent leads).

02_notebooks/

01_data_preprocessing_eda.ipynb — Data cleaning and market exploration.

02_classification_model.ipynb — Logistic Regression training & validation (AUC 0.74).

03_indian_market_forecast.ipynb — Z-Score alignment and 0.75 threshold application.

03_models/

abg_log_reg_model.pkl — Serialized Logistic Regression model.

abg_scaler.pkl — Saved Z-score scaler for cross-market consistency.

04_visuals/ — Tableau Dashboard (PDF) & Python strategic plots.

## 📈 Key Insights & Strategic Validation

1. Cross-Border Distribution Alignment (The Z-Score)
To account for the economic differences between Japan and India, I utilized Z-score Normalization. This ensured that "High Income" in India was mathematically aligned with the training data from Japan, allowing for a statistically sound forecast across different currencies.

2. Market Confidence Analysis
The "Double-Hump" Discovery: The probability distribution revealed a distinct "Premium Segment" (the spike at the far right).

The Decision: While many leads fall into the 50-60% range, I consciously bypassed this "Market Noise" to focus on the high-certainty cluster.

3. Threshold Optimization for ROI
Strategy: Using a conservative 0.75 probability threshold, I filtered the 70,000 leads down to the top 15,848 high-intent prospects.

Impact: This 0.75 "Passing Mark" ensures that ABG Motors prioritizes the most likely buyers, reducing potential marketing waste by ignoring low-confidence leads.

---
*Developed by Akash Tiwari | Data Analyst*
