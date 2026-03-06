# 🌾 AgroSentinel: Crop Failure Risk Analytics for Indian Agriculture
An end‑to‑end **data science and visualization project** that predicts and analyzes **crop failure risk** across Indian districts using real government datasets on crop production and climate parameters.  
Developed as part of **INT234 – Predictive Analytics**, this project combines machine learning, feature engineering, and interactive dashboards to produce actionable agricultural insights.

---

## 🚀 Features

✅ **1. Real Government Data Integration**  
- Crop production data from [data.gov.in](https://data.gov.in/catalog/district-wise-season-wise-crop-production-statistics-0)  
- Weather and rainfall data from the Indian Meteorological Department (IMD)  

✅ **2. Advanced Preprocessing Pipeline**  
- Cleaning, merging, and normalization of district‑wise agroclimatic data  
- Automated detection of outliers, missing value imputation, and categorical encoding  

✅ **3. Predictive Modelling**  
- Ensemble learning methods: Random Forest, XGBoost, Bagging, AdaBoost  
- Achieved **RMSE = 0.188 tons/ha** and **Accuracy = 89%** on validation  

✅ **4. Interactive Dashboard (Streamlit + Plotly)**  
- Dynamic filtering by state, crop, and season  
- Risk heatmaps, temporal yield trends, and correlation explorers  
- “What‑if” simulator to visualize risk impact when changing parameters  

✅ **5. Visual Reporting & Deployment**  
- Fully responsive **web dashboard** built with Plotly and Streamlit  
- Interactive results for real‑time decision‑making in farming and policy  

---

## 📁 Project Structure

crop_failure_project/
├── data/
│   └── crop_merged.csv          
├── app.py                      
├── notebooks/
│   └── crop_failure_prediction.ipynb  # Model training & EDA
├── models/
│   ├── rf_model.pkl
│   ├── xgb_model.pkl
│   └── scaler.pkl
├── visualizations/
│   ├── risk_heatmap.png
│   └── model_comparison.png
├── reports/
│   └── IEEE_final_report.pdf
└── README.md

## ⚙️ Installation

### Prerequisites
- Python ≥ 3.9  
- Git  
- pip (Python package installer)

### Setup Instructions

# Clone this repository

# Install dependencies
pip install -r requirements.txt

# Run dashboard locally
streamlit run app.py

## 🧩 Technologies Used

| Category | Tools/Frameworks |
|-----------|------------------|
| Programming | Python (Pandas, NumPy) |
| Machine Learning | scikit‑learn, XGBoost |
| Visualization | Plotly, Seaborn, Matplotlib |
| Web App | Streamlit |
| Data Sources | IMD, data.gov.in, DES |
| Storage | CSV datasets (local / online) |


## 🔍 Key Insights

- 🌧️ **Rainfall** is the most significant factor influencing yield (feature importance ~28%).  
- 🌾 **Wheat and Cotton** show highest variability across drought seasons.  
- 📉 **Rajasthan** districts exhibit a 38% failure rate, while **Tamil Nadu** maintains below 10%.  
- 🧮 Ensemble models outperformed linear models with better R² and lower RMSE.  
- 📈 Average yield increase of 12‑15% was found in districts with >60% irrigation coverage.


## 💡 Dashboard Highlights

| Dashboard Section | Description |
|--------------------|--------------|
| **Overview KPIs** | Total records, avg. yield, failure rate, district count |
| **EDA Visuals** | Distribution plots, correlation heatmaps, rainfall vs yield |
| **Risk Mapping** | Failure risk comparison by State × Crop × Season |
| **What‑If Simulator** | Interactive prediction using rainfall, temperature, soil, irrigation |
| **Model Summary** | RMSE and R² visualization for ensemble models |


## 🧠 Core Learning Objectives

1. Understand real‑world data preprocessing and feature engineering.  
2. Apply ensemble machine learning algorithms for regression and classification.  
3. Evaluate models using RMSE, R², accuracy, AUC.  
4. Visualize results through an interactive web‑based dashboard.  
5. Develop domain knowledge in agri‑tech and climate analytics.


## 📊 Model Performance

| Model | RMSE (tons/ha) | R² Score | Accuracy | AUC |
|--------|----------------|----------|-----------|-----|
| Random Forest | 0.214 | 0.82 | 87% | 0.91 |
| XGBoost | **0.188** | **0.88** | **89%** | **0.94** |
| Bagging | 0.224 | 0.79 | 86% | 0.89 |
| AdaBoost | 0.245 | 0.74 | 85% | 0.88 |

## 🌍 Future Scope

- Integration with **real‑time satellite & IoT weather sensors**  
- Implement **LSTM recurrent models** for time‑series yield forecasting  
- Add **district‑wise geospatial map** using folium or Mapbox  
- Build a **mobile‑first version** for farmer communities  
- Extend model training to include **economic and policy indicators**


## 📚 References

- [data.gov.in – Crop Production Statistics](https://www.data.gov.in/catalog/district-wise-season-wise-crop-production-statistics-0)  
- [IMD Pune – Rainfall and Climate Data](https://cdsp.imdpune.gov.in/home_gridded_data.php)  
- [India WRIS – Water and Irrigation Data](https://indiawris.gov.in)  
- [ICRISAT Data Portal](http://data.icrisat.org)


## 🧑‍💻 Author

UTSAH SINGH  
Data Scientist | ML Engineer | Researcher in Agri‑Analytics  
📍 Chandigarh, India  

## ⭐ How to Contribute

1. Fork the repository  
2. Create your feature branch (`git checkout -b feature/your-feature`)  
3. Commit changes (`git commit -m 'Add new analysis feature'`)  
4. Push to branch (`git push origin feature/your-feature`)  
5. Submit a Pull Request  

---

## 📜 License

This project is licensed under the **MIT License** — feel free to adapt, reuse, or modify with attribution.

---

**Built with ❤️ by Utsah Singh using Streamlit, Plotly & XGBoost**  
*"Empowering Indian Agriculture through Data‑Driven Insights."*


