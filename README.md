# 🎒 Backpack Price Prediction – Kaggle Playground Series S5E2

Welcome! This repository showcases my end-to-end solution for the **Backpack Price Prediction Challenge**, hosted on Kaggle as part of the Playground Series (Season 5, Episode 2). The objective was to build a regression model that accurately predicts the price of backpacks based on structured product features.

> 🏁 Achieved a **Public Leaderboard Rank** of **983 out of 3393 teams**  
> 📉 Final RMSE: **38.89951**  
> 💡 Model Used: **CatBoost Regressor**

---

## 📖 About the Challenge

Participants were given training and test data derived from a **deep learning model trained on the original Student Bag Prediction dataset**. Although feature distributions closely resembled the original dataset, they were not identical. The competition encouraged experimentation, including using the original dataset for comparison or performance improvement.

---

## 📂 Dataset Overview

| File Name             | Description                                                 |
|-----------------------|-------------------------------------------------------------|
| `train.csv`           | Main training dataset (includes `Price` target column)     |
| `train_extra.csv`     | Additional training samples provided                        |
| `test.csv`            | Test dataset for final predictions                          |
| `sample_submission.csv` | Submission format sample                                  |

📁 Full notebook and datasets are available here:  
🔗 [Google Drive Folder](https://drive.google.com/drive/folders/1dNbe7_uW4XctWeEScfHi3gTesT5qXVJi?usp=sharing)

---

## 🧠 Approach & Workflow

### 🧪 1. Exploratory Data Analysis (EDA)
- Investigated data distributions and types
- Compared `train.csv` and `train_extra.csv` to understand variations
- Identified key categorical features and missing values

### 🛠 2. Preprocessing
- Handled missing values using median and mode
- Avoided feature engineering to respect the competition’s integrity
- Leveraged **CatBoost’s native categorical handling** to simplify preprocessing

### 🤖 3. Modeling with CatBoost
- Used `CatBoostRegressor` for its:
  - Native support for categorical features
  - Built-in handling of missing data
  - Efficient training on tabular datasets
- Performed **5-Fold Cross-Validation** to ensure robust evaluation
- Trained final model using both `train.csv` and `train_extra.csv`

### 📈 4. Prediction & Submission
- Generated predictions on the test set
- Formatted results as per `sample_submission.csv`
- Uploaded final `submission.csv` to Kaggle

---

## 📦 Project Structure

