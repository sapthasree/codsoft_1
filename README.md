# codsoft_1

# Titanic Survival Prediction using Logistic Regression

This project was developed as part of my internship as a **Data Science Intern** at Codsoft.  
The goal was to apply fundamental data science techniques to predict passenger survival on the Titanic using machine learning.

## Dataset
The dataset used is the well-known **Titanic dataset**, containing details such as age, sex, ticket class, fare, and whether the person survived or not.

### Key Features:
- `Pclass`: Ticket class
- `Sex`: Gender
- `Age`: Age in years
- `SibSp`: Number of siblings/spouses aboard
- `Parch`: Number of parents/children aboard
- `Fare`: Ticket fare
- `Embarked`: Port of Embarkation
- `Survived`: Target variable (0 = No, 1 = Yes)

---

## Steps Performed

### 1. **Data Preprocessing**
- Dropped irrelevant columns: `PassengerId`, `Name`, `Ticket`, `Cabin`
- Handled missing values by dropping rows with missing `Age` and `Embarked`
- Encoded categorical features `Sex` and `Embarked` using Label Encoding

### 2. **Feature Selection**
- Chose relevant features as predictors (X)
- Chose `Survived` as the target variable (y)

### 3. **Model Building**
- Split data into train and test sets (80:20)
- Applied **Logistic Regression** using `sklearn`

### 4. **Model Evaluation**
- Predicted outcomes on the test set
- Compared actual vs predicted using a result matrix
- Calculated **accuracy**:  
  `Accuracy: 79.72%`

### 5. **Visualization**
- Plotted scatter plot of actual vs predicted values

---

## Libraries Used
```python
import pandas as pd
from sklearn.preprocessing import LabelEncoder
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LogisticRegression
from sklearn.metrics import accuracy_score
import matplotlib.pyplot as plt
```

---

## Output Sample

```plaintext
True Predicted
[[1 1]
 [1 1]
 ...
 [1 0]]
Accuracy: 79.72%
```

---

## Final Thoughts
This project reinforced my understanding of:
- Data cleaning and encoding
- Binary classification with logistic regression
- Accuracy evaluation and result interpretation

Looking forward to exploring more advanced models and contributing to real-world machine learning projects!

---

## Author
**Sapthasree N K**  
*Data Analyst Intern @ CodSoft .*
