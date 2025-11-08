# Titanic Machine Learning Baseline

A concise, reproducible project for the [Kaggle Titanic competition](https://www.kaggle.com/competitions/titanic).  
This repository demonstrates a simple end-to-end workflow for data exploration, feature engineering, model training, and submission generation using pandas and scikit-learn.

---

## Overview
The goal is to predict passenger survival based on demographic and travel features.  
This project provides a minimal, transparent starting point that can be extended into more advanced pipelines or model experiments.

---

## Directory Structure
```
titanic-ml/
├── data/              # raw train/test CSVs (not tracked by git)
├── notebooks/         # exploratory notebooks (EDA, experiments)
│   └── 01_eda_baseline.ipynb
├── src/               # main pipeline scripts
│   └── main.py
├── submissions/       # generated submission files
├── requirements.txt
├── .gitignore
└── README.md
```

---

## Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/titanic-ml.git
   cd titanic-ml
   ```

2. (Recommended) Create and activate a virtual environment:
   ```bash
   python -m venv .venv
   source .venv/Scripts/activate    # Git Bash
   # or
   .venv\Scripts\activate           # PowerShell / CMD
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Place the Kaggle `train.csv` and `test.csv` files in the `data/` directory.

---

## Usage
Run the training and prediction pipeline:
```bash
python src/main.py
```

The script will output:
```
submissions/submission.csv
```
Upload this file to Kaggle to get your first score.

---

## Next Steps
- Conduct exploratory analysis in `notebooks/01_eda_baseline.ipynb`.
- Refine feature engineering (e.g., handle missing values, extract titles, create family-based features).
- Experiment with different models (Logistic Regression, RandomForest, LightGBM, XGBoost).
- Add cross-validation for more robust validation performance.
- Log model results and version your experiments.

---

## License
MIT License
