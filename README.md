# House-Price-Prediction-On-User-Based-Inputs
ML-powered Jupyter notebook for predicting CA house prices from 20k+ dataset. Features: feature engineering, model training (Linear Reg, RF, XGBoost; R²~0.85), interactive user inputs for forecasts (e.g., $452K Bay Area home). EDA plots, saves, income-location insights. Colab-ready for portfolios!

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)](https://jupyter.org/)

**Predict house prices in California with interactive machine learning!** This Jupyter notebook leverages the classic California Housing dataset (20k+ records) to build, train, and compare regression models for accurate price forecasting. Input socioeconomic and geographic features—like median income, house age, rooms, and GPS coordinates—for instant predictions (e.g., "$452K" for a Bay Area home).

## 🚀 Quick Start

1. **Clone the Repo**:
   ```
   git clone https://github.com/yourusername/house-price-prediction.git
   cd house-price-prediction
   ```

2. **Install Dependencies**:
   ```
   pip install scikit-learn xgboost pandas numpy matplotlib seaborn joblib
   ```

3. **Run the Notebook**:
   - Open `PredictHousingPriceOnUserInput.ipynb` in Jupyter, JupyterLab, or Google Colab.
   - Execute all cells sequentially.
   - At the end, enter your house features via prompts for a personalized prediction!

4. **Use the Saved Model**:
   - Load `house_price_model.pkl` and `scaler.pkl` for standalone predictions.
   - Example: See the `predict_house_price()` function in the notebook.

## 🛠️ Key Features
- **Data Pipeline**: Loads dataset, engineers features (e.g., rooms per household), scales, and splits 80/20.
- **Models**: Linear Regression (baseline), Random Forest, Gradient Boosting, XGBoost (best: R² ~0.85).
- **Evaluation**: MAE/RMSE/R² metrics, comparison plots, residuals, and feature importance.
- **Interactive**: Validated user inputs with defaults; outputs price category and error estimates.
- **Visuals**: EDA (histograms, correlations), model comparisons, actual vs. predicted scatters.
- **Insights**: Median income (corr. 0.69) and coastal locations drive premiums.

## 📊 Results
- **Best Model**: XGBoost (R²: 0.85, MAE: ~$0.47K).
- **Sample Prediction**: For median income $80K, 35-year-old house with 6.5 rooms near SF—**$452,600** (Above Average category).

| Model          | R² Score | MAE ($100K) | RMSE ($100K) |
|----------------|----------|-------------|--------------|
| XGBoost       | 0.8500  | 0.472       | 0.621        |
| Random Forest | 0.8280  | 0.498       | 0.645        |
| Gradient Boost| 0.8120  | 0.521       | 0.672        |
| Linear Reg.   | 0.6120  | 0.652       | 0.810        |

## 📁 Files
- `PredictHousingPriceOnUserInput.ipynb`: Main notebook (EDA, training, predictions).
- `house_price_model.pkl`: Saved best model (XGBoost).
- `scaler.pkl`: Feature scaler for new data.

## 💡 Insights
- **Top Predictor**: Median income—higher earners correlate with pricier homes.
- **Location Matters**: Coastal latitudes (e.g., 37.8°) boost values by 20-30%.
- **Extend It**: Swap dataset for modern Zillow data or add neural nets!

## 🤝 Contributing
Fork, improve, and PR! Issues welcome.

## 📄 License
MIT License—feel free to use/modify. See [LICENSE](LICENSE) for details.

---

*Built with ❤️ for ML enthusiasts.*  
*(Last updated: Nov 2025)*
