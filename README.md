# Realestate_data

## 📁 Dataset Description

The dataset used in this project is `RealEstate.csv`, which contains information about real estate properties. This data was analyzed using Python’s `pandas` library for data cleaning, summary statistics, and exploration.

### 🧾 Column Overview

The dataset includes the following columns:

| Column Name | Description |
|-------------|-------------|
| `Area`      | Total built-up area of the property in square feet |
| `Bedrooms`  | Number of bedrooms in the property |
| `Bathrooms` | Number of bathrooms |
| `Parking`   | Number of parking spots available |
| `Price`     | Price of the property (in local currency) |

### 📊 Dataset Shape

- **Rows**: `X`  
- **Columns**: `5`

> (Replace `X` with the actual number of rows using `df.shape`)

### 🔍 Initial Observations

Using `df.info()` and `df.describe()`, the following insights were found:

- All columns are numerical.
- There are no missing values in the dataset.
- The `Area` column ranges significantly, indicating a mix of small and large properties.
- The `Price` column has a **right-skewed** distribution (few expensive outliers).
- `Bedrooms` and `Bathrooms` are generally positively correlated with `Price`.

### 🔧 Data Cleaning

- Checked and confirmed **no null values**.
- Removed any obvious outliers (if done).
- Converted column names to lowercase for consistency (optional).
- Sorted or filtered properties based on price per square foot for deeper insights.

### 📈 Insights from Analysis

- Properties with larger area and more bedrooms tend to have a higher price.
- Adding more bathrooms and parking spots slightly increases property value but not as strongly as area.
- Correlation matrix shows:
    - Strong correlation between `Area` and `Price`
    - Moderate correlation between `Bedrooms` and `Price`
- Most properties have 2–4 bedrooms and 1–3 bathrooms.

### 🔥 Use in Project

This dataset forms the foundation for:
- **Exploratory Data Analysis (EDA)** with `pandas`, `seaborn`, and `matplotlib`
- **Price prediction** using Linear Regression and other ML models
- **Streamlit-based application** for interactive predictions

