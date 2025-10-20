# tutorial-beginner-house-price-prediction
Repository นี้สร้างมาเพื่อเป็น guide ให้มือใหม่เข้าใจ process ของ ml เบื้องต้นอย่าง Regression ข้างล่างจะเป็นวิธี setup na krub

---


# 🏠 House Price Prediction Project

This project uses **Python + linear model + scikit-learn pipelines** to predict house prices based on multiple engineered features such as living area, lot size, renovation age, and more.  
It includes preprocessing pipelines, feature engineering, and trained machine learning models.

---

## ⚙️ Environment Setup

### 1️⃣ Clone the Repository
Went into your own selected directory and open the terminal 

````markdown
```bash
git clone https://github.com/Sakolkrit/tutorial-beginner-house-price-prediction.git
cd tutorial-beginner-house-price-prediction
````

---

### 2️⃣ Create a Virtual Environment (venv)

A virtual environment helps isolate project dependencies and prevents version conflicts.

#### 🪟 On Windows

```bash
python -m venv .venv(or other prference name on venv folder)
.venv\Scripts\activate
```

#### 🐧 On macOS / Linux

```bash
python3 -m venv .venv(or other prference name on venv folder)
source .venv/bin/activate
```

You should see something like `(.venv)` (or other name depend on how you named venv) in your terminal — that means it’s active ✅

---

### 3️⃣ Install Required Packages

Make sure you have the latest `pip`, then install all dependencies:

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

# Example input (raw data before feature engineering)

sample = pd.DataFrame([{
    "date": "2/5/2014  0:00:00",
    "bedrooms": 3,
    "bathrooms": 2,
    "floors": 1,
    "sqft_living": 1800,
    "sqft_lot": 5000,
    "sqft_above": 1600,
    "sqft_basement": 200,
    "yr_built": 1995,
    "yr_renovated": 0,
    "street": "123 6th Ave",
    "city": "Seattle",
    "statezip": "WA 98103",
    "country": "USA",
    "waterfront": 0,
    "view": 1,
    "condition": 3
}])

