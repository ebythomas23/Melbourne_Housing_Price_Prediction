# Melbourne Housing Analytics

## Overview
This project aims to predict housing median prices in Melbourne using historical data. By leveraging machine learning models, it provides actionable insights into market trends, supporting decision-making for stakeholders like real estate agents, investors, and policymakers.

## Key Features
- **Exploratory Data Analysis (EDA):** Gained insights into Melbourne's housing trends.
- **Feature Engineering:** Incorporated rolling averages and transaction density for improved predictions.
- **Machine Learning Models:**
  - Baseline: Linear Regression.
  - Advanced: Tuned Random Forest Regressor.
- **Performance Metrics:** Focused on RMSE and R² scores to evaluate model effectiveness.

---

## Repository Structure
```plaintext
Melbourne_Housing_Analytics/
├── README.md               # High-level overview of the project
├── data/                   # Dataset folder
│   ├── raw/                # Raw datasets
│   │   └── house-prices-by-small-area-sale-year.csv
│   ├── processed/          # Cleaned and feature-engineered datasets
│       └── enhanced_data.csv
├── models/                 # Saved models
│   └── best_model.pkl
├── notebooks/              # Jupyter notebooks for each step
│   ├── 01_data_preprocessing.ipynb
│   ├── 02_exploratory_data_analysis.ipynb
│   ├── 03_feature_engineering.ipynb
│   ├── 04_modelling.ipynb
├── reports/                # Polished reports
│   └── housing_market_report.pdf
├── visuals/                # Plots and visualizations
│   ├── residual_plot.png
│   └── feature_importance_plot.png
├── requirements.txt        # Python dependencies

```

# How to Run

## Clone the Repository
```bash
git clone <repo_url>
cd Melbourne_Housing_Analytics
```
## Set Up the Environment
Install the required dependencies:
```bash
pip install -r requirements.txt
```
## Explore Notebooks
Launch Jupyter Notebook to explore the workflow:
```bash
jupyter notebook notebooks/01_data_preprocessing.ipynb
```

## Results

### Model Performance
| **Model**              | **Test RMSE** | **Test R²** |
|-------------------------|---------------|-------------|
| Linear Regression       | 276,091       | 0.519       |
| Random Forest (Tuned)   | 197,573       | 0.754       |

### Key Insights
1. The tuned Random Forest model significantly outperformed the Linear Regression model:
   - **28% reduction** in RMSE.
   - Explained **75.4%** of the variance in housing prices.
2. **Feature Importance:**
   - Rolling average price: Most significant predictor.
   - Transaction density: Second most important feature.

### Visualizations
- ![Residual Plot](visuals/residual_plot.png)
- ![Feature Importance](visuals/feature_importance_plot.png)

---

## Report
A detailed report summarizing the project's methodology and findings:
- [Housing Market Report (PDF)](reports/housing_market_report.pdf)

---

## Future Enhancements
1. **Expand Features:** Include socioeconomic and environmental data for better predictions.
2. **Handle Outliers:** Investigate high-residual cases to improve accuracy.
3. **Deployment:** Build a dashboard or API for real-time predictions.
4. **Extend Analysis:** Apply the methodology to other cities or regions.

---

## Acknowledgments
- **Data Source:** [City of Melbourne Open Data](https://data.melbourne.vic.gov.au).
- **Tools:** Python (Pandas, Scikit-learn, Matplotlib, Seaborn).

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

