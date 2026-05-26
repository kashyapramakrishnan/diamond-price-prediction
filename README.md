# 💎 Diamond Price Prediction

A machine learning project that predicts diamond prices using features such as carat, cut, color, clarity, and physical dimensions. Built using Python, data analysis libraries, and regression models.

---

## 📌 Project Overview

This project focuses on:

* Data cleaning and preprocessing
* Exploratory Data Analysis (EDA)
* Handling skewed distributions and outliers
* Feature engineering and encoding
* Training and evaluating regression models
* Predicting diamond prices with improved accuracy

The notebook walks through the complete machine learning workflow from raw dataset to final model evaluation.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* SciPy

---

## 📂 Dataset Features

| Feature | Description                           |
| ------- | ------------------------------------- |
| carat   | Weight of the diamond                 |
| cut     | Quality of the cut                    |
| color   | Diamond color grade                   |
| clarity | Diamond clarity grade                 |
| depth   | Total depth percentage                |
| table   | Width of top relative to widest point |
| x       | Length in mm                          |
| y       | Width in mm                           |
| z       | Depth in mm                           |
| price   | Target variable                       |

---

## 🔍 Data Preprocessing

The following preprocessing steps were performed:

* Removed duplicate rows
* Checked and handled invalid dimension values (`x`, `y`, `z` = 0)
* Detected and removed extreme outliers using the IQR method
* Performed normality checks
* Applied log transformation to the target variable (`price`) to reduce skewness
* Encoded ordinal categorical features (`cut`, `color`, `clarity`)
* Performed correlation analysis and feature selection
* Standardized numerical features

---

## 📊 Exploratory Data Analysis

EDA included:

* Distribution plots
* Correlation heatmaps
* Outlier visualization
* Normality analysis
* Feature relationship analysis

The project also investigates multicollinearity between dimensions (`x`, `y`, `z`) and `carat`.

---

## 🤖 Machine Learning Models

The notebook trains and evaluates regression models for price prediction.

Evaluation metrics include:

* MAE (Mean Absolute Error)
* RMSE (Root Mean Squared Error)
* R² Score

---

## 📈 Key Insights

* Diamond price distribution is highly right-skewed
* Log transformation significantly improves target distribution
* `carat` has the strongest influence on price
* Physical dimensions are highly correlated with carat
* Proper preprocessing greatly improves model performance

---

## 🚀 How to Run

1. Clone the repository

```bash
git clone https://github.com/kashyapramakrishnan/diamond-price-prediction.git
```

2. Navigate to the project folder

```bash
cd diamond-price-prediction
```

3. Install dependencies

```bash
pip install -r requirements.txt
```

4. Run the Jupyter Notebook

```bash
jupyter notebook
```

---

## 📁 Project Structure

```text
├── diamonds_price_prediction_final.ipynb
├── diamonds_data.csv
├── README.md
└── requirements.txt
```

---

## 🎯 Future Improvements

* Hyperparameter tuning
* Model deployment using Flask or Streamlit
* Cross-validation optimization
* Trying ensemble models
* Building an interactive prediction dashboard

---

## 👤 Authors

Kashyap Ramakrishnan
Swetha V Gopal

M.Sc Applied Statistics and Data Analytics Students
Amrita Vishwa Vidyapeetham, Coimbatore

If you found this project useful, consider starring the repository. Tiny bursts of dopamine are basically the fuel source of open-source development.
