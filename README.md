# Insurance Cost Prediction using Machine Learning

## 📌 Project Overview
This project focuses on **analyzing and predicting medical insurance costs** using demographic and lifestyle data. It combines **Exploratory Data Analysis (EDA)** with **machine learning models** to understand key cost drivers and build predictive models.

The dataset includes features such as age, BMI, smoking status, number of children, and region to predict insurance charges.

---

## 📂 Project Structure

mini-project-1/
├── data/
│   └── insurance.txt
├── notebooks/
│   ├── 01_exploration.ipynb
│   └── 02_modeling.ipynb
├── requirements.txt
└── README.md


---

## 📊 Dataset Description
The dataset contains **1338 records** with the following features:

| Column     | Description |
|------------|------------|
| age        | Age of the individual |
| sex        | Gender (male/female) |
| bmi        | Body Mass Index |
| children   | Number of children |
| smoker     | Smoking status (yes/no) |
| region     | Residential region |
| charges    | Medical insurance cost (target variable) |

✔ No missing values  
✔ No duplicate rows  

---

## 🔍 Exploratory Data Analysis (EDA)
Performed in **`cost_insurance.ipynb`**, including:

- Distribution analysis of insurance charges  
- Boxplots for:
  - Smoker vs Charges
  - Sex vs Charges
  - Region vs Charges
- Scatter plots:
  - Age vs Charges (by smoker status)
  - BMI vs Charges with obesity threshold
- Correlation heatmap

### 🔑 Key Insights
- Smoking has the **strongest impact** on insurance costs  
- Higher BMI and age generally lead to higher charges  
- Non-smokers have significantly lower medical costs  

---

## ⚙️ Data Preprocessing
Performed in **`modeling.ipynb`**:
- Binary encoding for:
  - `sex`
  - `smoker`
- One-hot encoding for:
  - `children`
  - `region`
- Feature scaling using:
  - `StandardScaler`
- Train-test split (70% training, 30% testing)

---

## 🤖 Machine Learning Models
The following regression models were trained and evaluated:

- **Ordinary Least Squares (Linear Regression)**
- **Ridge Regression (L2)**
- **Lasso Regression (L1)**

### 📈 Model Performance (R² Score)

| Model | R² Score |
|------|---------|
| Linear Regression | ~0.759 |
| Ridge Regression | ~0.759 |
| Lasso Regression | ~0.759 |

All models perform similarly, indicating a strong linear relationship between features and insurance charges.

---

## 🛠️ Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab

---

## 🚀 How to Run the Project
1. Clone the repository:
   ```bash
   git clone https://github.com/Tanishq200307/mini-project-1

Open notebooks in Google Colab or Jupyter Notebook

Ensure insurance.csv is in the same directory

Run cells sequentially

📌 Future Improvements

Try non-linear models (Random Forest, XGBoost)

Feature engineering (interaction terms)

Hyperparameter tuning

Model deployment using Flask or FastAPI

👤 Author

Tanishq Rawat
Data Analysis & Machine Learning Enthusiast

