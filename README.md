# Student Performance Indicator - End to End Machine Learning Project

This project analyzes and predicts student performance based on various factors such as gender, ethnicity, parental education, lunch type, and test preparation. It demonstrates a complete machine learning workflow, from data exploration to model deployment.

## Table of Contents

- [Project Structure](#project-structure)
- [Dataset](#dataset)
- [Features](#features)
- [How to Run](#how-to-run)
- [Notebooks](#notebooks)
- [Deployment](#deployment)
- [Results & Insights](#results--insights)
- [Author](#author)

---

## Project Structure

```
├── application.py                # Main application script (Flask app)
├── requirements.txt              # Project dependencies
├── setup.py                      # Project packaging configuration
├── .gitignore
├── .ebextensions/                # AWS Elastic Beanstalk config
│   └── python.config
├── artifacts/                    # Data and model artifacts
│   ├── data.csv
│   ├── model.pkl
│   ├── preprocessor.pkl
│   ├── raw.csv
│   ├── test.csv
│   └── train.csv
├── catboost_info/                # CatBoost training logs
├── logs/                         # Log files for runs
├── mlproject.egg-info/           # Packaging metadata
├── notebook/                     # Jupyter notebooks for EDA and model training
│   ├── 1 . EDA STUDENT PERFORMANCE .ipynb
│   └── 2. MODEL TRAINING.ipynb
├── src/                          # Source code (modules, utils, etc.)
├── templates/                    # HTML templates for web app
│   └── home.html
└── README.md
```

## Dataset

- Source: [Kaggle - Students Performance in Exams](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams?datasetId=74977)
- 1000 rows, 8 columns:
  - gender
  - race/ethnicity
  - parental level of education
  - lunch
  - test preparation course
  - math score
  - reading score
  - writing score

## Features

- **Exploratory Data Analysis (EDA):** In-depth analysis of student performance and feature relationships.
- **Data Preprocessing:** Handling missing values, encoding, feature engineering.
- **Model Training:** Linear Regression and other models for predicting scores.
- **Evaluation:** Metrics such as RMSE, MAE, R2.
- **Deployment:** Flask web app for predictions, AWS Elastic Beanstalk ready.

## How to Run

1. **Clone the repository:**
   ```sh
   git clone <repo-url>
   cd ML-Projects
   ```

2. **Install dependencies:**
   ```sh
   pip install -r requirements.txt
   ```

3. **Run the application:**
   ```sh
   python application.py
   ```

4. **Access the web app:**  
   Open your browser at `http://localhost:5000`

## Notebooks

- [notebook/1 . EDA STUDENT PERFORMANCE .ipynb](notebook/1%20.%20EDA%20STUDENT%20PERFORMANCE%20.ipynb): Exploratory Data Analysis
- [notebook/2. MODEL TRAINING.ipynb](notebook/2.%20MODEL%20TRAINING.ipynb): Model training and evaluation

## Deployment

- AWS Elastic Beanstalk configuration is provided in `.ebextensions/`.
- Artifacts and logs are stored in `artifacts/` and `logs/`.

## Results & Insights

- Female students tend to perform better overall, but males score higher in math.
- Parental education and lunch type significantly affect performance.
- Completing the test preparation course improves scores.

## Author

- **Tejas Kamble**  
  [tejaskamble1018@gmail.com](mailto:tejaskamble1018@gmail.com)

---

> This project demonstrates a full ML workflow: EDA, preprocessing, modeling, evaluation, and deployment.