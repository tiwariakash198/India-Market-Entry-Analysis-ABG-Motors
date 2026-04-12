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

├── 01_data/
│   ├── 01_raw/                   # Unprocessed Japanese & Indian datasets
│   ├── 02_processed/             # Cleaned Japanese & Indian datasets
│   └── 03_forecasted_results/    # Final prediction output (15,848 leads)
├── 02_notebooks/
│   ├── 01_data_preprocessing_eda  # Data cleaning and market exploration
│   ├── 02_classification_model   # Logistic Regression training & validation
│   └── 03_indian_market_forecast # Applying model to Indian lead set
├── 03_models/
│   ├── car_buyer_model.pkl       # Serialized Logistic Regression model
│   └── scaler.pkl                # Saved Z-score scaler for consistency
├── 04_visuals/                   # Tableau Dashboard (PDF) & Python trend plots
└── README.md                     # Project overview and executive summary

## 📈 Key Insights
1.  **Affordability Correlation:** Purchase probability scales linearly with annual income, peaking at **70%+** for the >1.5M INR segment.
2.  **Replacement Cycle:** A significant "Upgrade Window" was identified for vehicles aged **more than a year (360+ days)**.
3.  **Risk Mitigation:** Applied a conservative **75% probability threshold** to ensure the forecast remains grounded in high-intent buyer behavior.

---
*Developed by Akash Tiwari | Data Analyst*