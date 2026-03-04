# 🏠 House Price Prediction System — Gurgaon

> An end-to-end machine learning project to predict residential property prices in Gurgaon, India — covering data collection, EDA, feature engineering, model selection, and a property recommender system.

---

## 📁 Project Structure

```
House-Price-Prediction/
│
├── 📓 Notebooks (in order)
│   ├── 1. eda-multivariate-analysis.ipynb
│   ├── 2. data-preprocessing.ipynb
│   ├── 3. merge-flats-and-house.ipynb
│   ├── 4. data-preprocessing-2.ipynb
│   ├── 5. feature-engineering.ipynb
│   ├── 6. eda-univariate-analysis.ipynb
│   ├── 7. eda-multivariate-analysis.ipynb
│   ├── 7. eda-pandas-profiling.ipynb
│   ├── 8. eda-multivariate-analysis.ipynb
│   ├── 9. outlier-treatment.ipynb
│   ├── 10. missing-value-imputation.ipynb
│   ├── 11. feature-selection.ipynb
│   ├── 12. feature-selection.ipynb
│   ├── 13. baseline-model.ipynb
│   ├── 14. model-selection.ipynb
│   ├── data-visualization.ipynb
│   ├── insights-module.ipynb
│   └── recommender-system.ipynb
│
├── 📊 Data
│   ├── apartments.csv
│   ├── flats.csv
│   ├── flats_cleaned.csv
│   ├── houses.csv
│   ├── house_cleaned.csv
│   ├── latlong.csv
│   ├── gurgaon_properties.csv
│   ├── gurgaon_properties_cleaned_v1.csv
│   ├── gurgaon_properties_cleaned_v2.csv
│   ├── gurgaon_properties_missing_...csv
│   ├── gurgaon_properties_outlier_...csv
│   └── gurgaon_properties_post_...csv
│
├── 🤖 Models
│   ├── df.pkl
│   └── pipeline.pkl
│
└── 📄 output_report.html
```

---

## 🔄 Pipeline Overview

```
Raw Data (Flats + Houses)
        ↓
   Data Merging
        ↓
 Preprocessing & Cleaning
        ↓
Outlier Treatment & Missing Value Imputation
        ↓
  Feature Engineering
        ↓
   Feature Selection
        ↓
  Baseline Modelling
        ↓
   Model Selection  ──→  pipeline.pkl
        ↓
Analytics + Recommender System
```

---

## 🧠 Key Steps

### 1. Data Collection & Merging
- Scraped and merged **flats** and **houses** data from Gurgaon listings
- Unified schema across property types

### 2. Exploratory Data Analysis
- Univariate & Multivariate analysis
- Pandas Profiling report (`output_report.html`)
- Correlation heatmaps, distribution plots, geo-visualizations

### 3. Data Preprocessing
- Handling missing values with imputation strategies
- Outlier detection and treatment
- Data type fixes and schema normalization

### 4. Feature Engineering
- Derived features: price per sqft, property age, BHK type, etc.
- Latitude/Longitude integration from `latlong.csv`
- Encoding categorical variables

### 5. Feature Selection
- Correlation-based filtering
- Variance Inflation Factor (VIF) analysis
- Importance-based selection

### 6. Model Building & Selection
- Baseline model benchmarking
- Compared multiple regressors (Linear Regression, Ridge, Random Forest, XGBoost, etc.)
- Final model exported as `pipeline.pkl`

### 7. Recommender System
- Property recommendation based on user preferences and similarity scores

---

## 🛠️ Tech Stack

| Category | Tools |
|---|---|
| Language | Python 3.x |
| Data Manipulation | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn, Plotly |
| EDA | Pandas Profiling / ydata-profiling |
| ML Models | Scikit-learn, XGBoost |
| Geo Analysis | Folium / Lat-Long data |
| Serialization | Pickle |
| Notebooks | Jupyter Notebook |

---

## ⚙️ Setup & Usage

```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/house-price-prediction.git
cd house-price-prediction

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run notebooks in order (1 → 14)
jupyter notebook
```

---

## 📈 Results

| Model | R² Score | RMSE |
|---|---|---|
| Linear Regression | — | — |
| Random Forest | — | — |
| XGBoost | — | — |

> *(Fill in your actual scores after running `14_model_selection.ipynb`)*

---

## 📌 Dataset

- **Source**: Gurgaon real estate listings (scraped/collected)
- **Features**: Location, Area (sqft), BHK, Bathrooms, Floor, Property Age, Amenities, etc.
- **Target**: Property Price (INR)

---

## 👤 Author

**Akash Kar** — B.Tech Biomedical Engineering, NIT Rourkela  
🔗 [LinkedIn](https://www.linkedin.com/in/akash-kar-0a7a7826a/) | [GitHub](https://github.com/Akashkar00)

---

## 📄 License

This project is open-source under the [MIT License](LICENSE).
