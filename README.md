# Real-Estate-prediction


This project performs an exploratory data analysis (EDA) on the Seattle house price dataset (`kc_house_data.csv`). The notebook is designed for use in **Google Colab** and walks through data cleaning, feature engineering, and insightful visualizations to understand the factors affecting housing prices.

## 📊 Overview

The notebook provides:
- Data loading and preprocessing
- Feature engineering for housing age and renovations
- Exploratory visualizations using **Seaborn**, **Matplotlib**, and **Plotly**
- Geospatial insights using latitude/longitude
- Correlation heatmaps to identify key factors influencing price

## 🧰 Technologies Used

- Python 3.x
- Pandas & NumPy
- Seaborn & Matplotlib
- Plotly Express
- Google Colab environment

## 📁 Dataset

- **Source**: `kc_house_data.csv`
- This dataset includes home sales data for King County, including Seattle. It has 21,613 rows and 21 columns (e.g., price, bedrooms, bathrooms, sqft, location, etc.)

## 🧪 Main Steps

### 1. Data Loading
- Uploading the CSV via Colab’s `files.upload()`.
- Parsing the `date` column into datetime format.
- Dropping irrelevant columns like `id`.

### 2. Feature Engineering
- Replacing 0s in `yr_renovated` with NaNs.
- Creating new features:
  - `house_age`
  - `years_since_renovation`
  - `price_per_sqft`

### 3. Visualizations
- **Histogram** of house prices.
- **Heatmap** of correlation between numeric features.
- **Scatter plot** of price vs. living area (`sqft_living`).
- **Boxplot** comparing price across bedroom counts.
- **Geospatial heatmap** of price distribution using `latitude` and `longitude`.

## 📸 Example Visualizations

- 📈 Price distribution reveals right-skewed pricing
- 📊 High correlation between `sqft_living` and price
- 🗺️ Heatmap shows higher prices concentrated in certain geographic areas

## 🚀 How to Run

1. Open the notebook in [Google Colab](https://colab.research.google.com/)
2. Upload `kc_house_data.csv` when prompted
3. Run all cells sequentially

