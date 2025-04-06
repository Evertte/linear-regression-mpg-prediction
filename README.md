# Linear Regression MPG Prediction 🚗📈

This project uses **Linear Regression** to predict a car's **miles per gallon (MPG)** based on features like horsepower, weight, age, and origin. It demonstrates a practical application of regression using real-world automotive data.

---

## 🔍 Overview

- Predicts fuel efficiency (MPG) using numerical vehicle attributes
- Built using Python with scikit-learn
- Covers data preprocessing, training, evaluation, and prediction

---

## 📊 Sample Dataset

| mpg  | cylinders | horsepower | weight | age | origin_japan | origin_usa |
|------|-----------|------------|--------|-----|--------------|------------|
| 18.0 | 8         | 130.0      | 3504   | 55  | 0            | 1          |
| 15.0 | 8         | 165.0      | 3693   | 55  | 0            | 1          |
| 18.0 | 8         | 150.0      | 3436   | 55  | 0            | 1          |
| 16.0 | 8         | 150.0      | 3433   | 55  | 0            | 1          |
| 17.0 | 8         | 140.0      | 3449   | 55  | 0            | 1          |

---

## 📈 Model Performance

- **R² Score**: 0.78
- **Mean Squared Error (MSE)**: 11.24
- **Mean Absolute Error (MAE)**: 2.52
- **Intercept**: 80.58

The model explains ~78% of the variance in MPG, making it a reliable tool for estimating fuel efficiency.

---

## 🧪 Example Usage

```python
import numpy as np
from sklearn.linear_model import LinearRegression

# Assume lm_model is your trained LinearRegression model
new_data = np.array([[8, 150, 3500, 55, 1, 0]])  # [cylinders, horsepower, weight, age, origin_japan, origin_usa]
predicted_mpg = lm_model.predict(new_data)
print("Predicted MPG:", predicted_mpg[0])
```

**Output:**
```
Predicted MPG: 17.54
```

---

## ⚙️ Technologies Used

- Python 3
- Pandas
- NumPy
- scikit-learn
- Matplotlib
- Seaborn

---

## ✨ Future Improvements

- Add regularization (Ridge, Lasso)
- Use cross-validation for model robustness
- Deploy as a web app using Flask or Streamlit

---
