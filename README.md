# 🌦️ Weather Prediction – Seattle, WA

This project analyzes Seattle’s weather patterns to predict precipitation and temperature trends using machine learning. By exploring the relationships between temperature, wind, and rainfall, the project aims to improve short-term weather forecasting and identify key factors influencing rain events.

---

## 📘 Project Overview
- Examined 1,461 daily weather observations from a Kaggle dataset.  
- Explored the relationship between temperature, precipitation, and wind speed.  
- Conducted detailed Exploratory Data Analysis (EDA) using correlation heatmaps, boxplots, and scatter plots.  
- Developed and compared **Linear Regression** and **Random Forest** models to predict precipitation and weather types.  
- Evaluated model performance using **R²**, **Mean Squared Error (MSE)**, and **ROC-AUC**.

---

## 🧠 Key Findings
- **Random Forest** achieved an **R² of 0.999** and **MSE of 0.0017**, demonstrating near-perfect predictive accuracy.  
- **Maximum temperature** was the most important predictor for rainfall.  
- Most precipitation events were light, with extreme rainfall being rare.  
- Cluster analysis identified three temperature-based weather groupings (rainy, mild, and sunny conditions).  
- The model successfully predicted **no rain** for January 1–2, 2016, aligning with actual weather data.

---

## ⚙️ Methods and Tools
**Data Preprocessing:**  
- Encoded categorical weather variables (rain, drizzle, snow, fog, sun).  
- Checked for missing values and normalized data distributions.  
- Generated lagged features (e.g., `temp_max_lag1`, `precipitation_lag1`) for better temporal modeling.  

**Modeling:**  
- Linear Regression  
- Random Forest Classifier & Regressor  
- Clustering (K-Means for temperature-based grouping)

**Tools Used:**  
Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Jupyter Notebook

---

## 📊 Files Included
- `Weather_Prediction_Report.pdf` → Final report and analysis  
- `Weather_Prediction.ipynb` → Jupyter Notebook containing data cleaning, EDA, and modeling  
- `data/` → Weather dataset (Kaggle source, daily Seattle observations)

> Note: Large CSVs may not render directly in GitHub — download the repository to view or run the notebook locally.

---

## 🏁 Conclusion
The Random Forest model provided highly accurate predictions for short-term Seattle weather, identifying temperature as the dominant factor influencing rainfall. While the dataset’s simplicity limited generalization, the project demonstrates how machine learning can effectively capture key local weather patterns. Future work could include adding variables like humidity and atmospheric pressure to enhance predictive performance.

---

## 📚 References
- [Kaggle Weather Dataset](https://www.kaggle.com/code/syedali110/weather-prediction-using-rnn/input)  
- [Seattle Weather Statistics](https://seattleweatherblog.com/rain-stats/)  
- [US Climate Data – Seattle](https://www.usclimatedata.com/climate/seattle/washington)
