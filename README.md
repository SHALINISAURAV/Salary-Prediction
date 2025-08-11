# Salary Prediction using Linear Regression

This project predicts the salary of an employee based on their years of experience using **Simple Linear Regression**.

## 📌 Project Overview
The aim of this project is to demonstrate the basic concepts of **Machine Learning Regression** by building a predictive model that estimates salaries from years of experience.

**Algorithm Used:** Linear Regression (Supervised Learning - Regression)  
**Programming Language:** Python  
**Libraries Used:** pandas, matplotlib, scikit-learn, pickle

---

## 📂 Dataset
The dataset `Salary_Data.csv` contains two columns:
- `YearsExperience` → Independent variable (Feature)
- `Salary` → Dependent variable (Target)

Example:
| YearsExperience | Salary   |
|-----------------|----------|
| 1.1             | 39343    |
| 1.3             | 46205    |
| 1.5             | 37731    |

---

## ⚙️ How It Works
1. **Data Loading**: The CSV file is read using `pandas`.
2. **Data Splitting**: The dataset is split into **training** and **testing** sets.
3. **Model Training**: A Linear Regression model is trained on the training set.
4. **Model Evaluation**: The model is tested using the testing set.
5. **Visualization**: The best fit line is plotted against the training data.
6. **Model Saving**: The trained model is saved as a `.pkl` file for future use.

---

## 📊 Model Performance
- **Slope (m)**: Represents salary increment per year of experience.
- **Intercept (c)**: Base salary when experience is 0.
- **R² Score**: Indicates how well the model fits the data.
- **Mean Absolute Error**: Average difference between predicted and actual salary.

---

## 🛠 Installation & Usage

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/salary-prediction.git
cd salary-prediction
```

### 2. Install Dependencies
```bash
pip install pandas matplotlib scikit-learn
```

### 3. Run the Script
```bash
python salary_prediction.py
```

### 4. Load the Model (Optional)
```python
import pickle
model = pickle.load(open('salary_model.pkl', 'rb'))
print(model.predict([[5]]))  # Predict salary for 5 years of experience
```

---

## 📷 Visualization
The project also plots:
- Training Data (Blue)
- Testing Data (Green)
- Best Fit Regression Line (Red)

---

## 📌 Concepts Learned
- Supervised Learning
- Regression Analysis
- Train-Test Split
- Model Evaluation Metrics (R² Score, MAE)
- Model Serialization (Pickle)

---

## 📜 License
This project is licensed under the MIT License.
