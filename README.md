# 🏡 RealtyVision – AI-Powered Real Estate Insights and Predictions

![Streamlit](https://img.shields.io/badge/Built%20with-Streamlit-orange)
![Python](https://img.shields.io/badge/Language-Python-blue)
![ML](https://img.shields.io/badge/Machine%20Learning-Yes-green)

---

## 📌 Project Objective

**RealtyVision** is a data-driven, AI-powered web application designed to help users make informed decisions in the real estate market. It predicts property prices based on key features, recommends similar properties, and provides visual insights into real estate trends, leveraging data scraped from [99acres](https://www.99acres.com/).

---

## 🧠 Features

🔹 **Analytical Module**  
> Provides city-level insights, price distributions, and real estate market trends using interactive visualizations.

🔹 **Price Prediction Module**  
> Allows users to input property features and get instant price predictions using trained machine learning models.

🔹 **Recommender System**  
> Suggests similar properties based on user-input criteria using a content-based recommendation engine.

🔹 **Insight Module**  
> Explains the contribution of each feature (e.g., location, area, BHK) to the final predicted price using SHAP (Shapley Additive Explanations).

---

## 🛠 Tech Stack

| Component       | Technology Used              |
|----------------|------------------------------|
| Language        | Python                       |
| Frontend UI     | Streamlit                    |
| Data Handling   | Pandas, NumPy                |
| Web Scraping    | BeautifulSoup, Requests      |
| ML Models       | LightGBM, Random Forest, Linear Regression |
| Recommender     | Cosine Similarity (Scikit-learn) |
| Visualization   | Matplotlib, Plotly, Seaborn  |
| Model Explainability | SHAP                   |

---

## 🔄 Machine Learning Lifecycle

### 1. **Data Collection**
- Scraped structured housing data from 99acres using BeautifulSoup.

### 2. **Preprocessing**
- Cleaned data, handled nulls, removed outliers, encoded categories.

### 3. **Feature Engineering**
- Created derived features like `price_per_sqft`, `amenity_count`, etc.

### 4. **Model Training**
- Tried multiple regressors:  
  - Linear Regression  
  - Random Forest  
  - **LightGBM** *(selected due to lowest RMSE)*

### 5. **Evaluation Metrics**
- RMSE (≈ ₹20 Lakhs)
- MAE
- R² Score
- 5-Fold Cross Validation

### 6. **Model Explainability**
- Used SHAP values to interpret model decisions at both global and individual prediction levels.

---

## 📊 Sample Visualizations

- 📍 City-wise price trend heatmaps  
- 🧮 Price distribution histograms  
- 📌 SHAP summary and force plots  
- 🏙️ Recommender output showing similar properties

---

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/realtyvision.git
   cd realtyvision
   ```
