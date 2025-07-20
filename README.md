# 🌾 Crop Yield Prediction Using Machine Learning
Full report and notebook can be accessed in this repository.

## 🌱 Project Overview
Crop yield is influenced by a variety of environmental and agronomic factors. This project uses supervised machine learning to predict crop yields in ASEAN countries using:
- 📈 Historical yield data  
- ☀️ Temperature  
- 🌧️ Precipitation  
- 🧪 Pesticide usage

The goal is to help farmers and agricultural stakeholders make data-driven decisions to increase productivity and sustainability.

## 📊 Dataset Sources
- **Yield & Pesticides**: FAO (2025)  
- **Precipitation**: Our World in Data (2025)  
- **Temperature**: Kaggle (Palinatx, 2024)

## 🧠 Methodology
- **Exploratory Data Analysis**: Outlier detection, correlation analysis, and yield distribution by crop & country
- **Encoding**:
  - One-hot encoding for `Country`
  - Target encoding for `Crop`
- **Scaling**: Min-Max scaling
- **Train/Test Splits**: Evaluated 80/20, 90/10, and 95/5

## 🛠️ Models Applied
- 🌲 Random Forest Regressor  
- 🔺 Gradient Boosting Regressor  
- ⚡ XGBoost Regressor  
- 🧠 Ridge Regression  
- 🧊 K-Nearest Neighbors  
- 📉 Support Vector Regressor (did not perform well)

## 🧪 Evaluation Metrics
- **R² Score**: Goodness of fit  
- **RMSE**: Error in predicted yield values

> Final selected split: **80/20**  
> Final selected model: **Gradient Boosting Regressor (94% R² score)**

## 🔍 Key Insights
- **Top Crops**: Sugarcane, Pineapples, Papayas
- **Top Rice Yield Countries**: Vietnam, Indonesia
- **Environmental Impact**: Precipitation moderately affects pesticide use; yield correlation varies by crop
- **Gradient Boosting Regressor** was selected for its balance and better emphasis on feature relevance (less bias toward country)

## 🔧 Tools & Libraries
- Python (pandas, scikit-learn, matplotlib, seaborn, XGBoost)
- Jupyter Notebook
- GridSearchCV for hyperparameter tuning

## 📈 Future Improvements
- Integrate real-time satellite or soil data  
- Try neural networks or time-series models  
- Extend to non-ASEAN regions
