# Week 5 Lab — Data Preprocessing (PROG8245)

This repo contains my Week 4 lab work on **data tidying, data cleaning, missing value imputation, and outlier detection** using four small practice datasets.

---

## What’s inside (quick summary)
- **PEW dataset:** practice reshaping a “wide” table into a tidy format using `melt`.
- **Billboard dataset:** more tidying + string cleaning (weekly ranks → tidy rows).
- **Cars dataset:** data cleaning + handling missing values (drop vs impute using `SimpleImputer`).
- **Diabetes dataset:** outlier detection using plots + **Z-score** and **IQR**, and then removing outliers.

---

## Dataset sources (what I used)
- **PEW (Religion vs Income):** a common “tidy data” teaching example used in many data-wrangling tutorials (Pew-style crosstab format).
- **Billboard weekly rankings:** a popular teaching dataset format where weekly columns need reshaping into tidy rows.
- **Cars dataset:** workshop-provided practice dataset (similar to Auto/MPG-style datasets used for cleaning/imputation examples).
- **Diabetes dataset:** workshop-provided practice dataset (typical health-feature columns used for outlier detection practice).

> Note: These CSVs were provided/used for learning in this lab. The goal is practicing the preprocessing techniques, not building a final ML model.

---

## Project structure
```
Week5/
├─ data/
│  └─ raw/
│     ├─ pew_dataset.csv
│     ├─ billboard_dataset.csv
│     ├─ cars_dataset.csv
│     └─ diabetes_dataset.csv
├─ week5Lab.ipynb
├─ requirements.txt
└─ .gitignore
```

---

## Setup (recommended)
### 1) Create and activate a virtual environment
**Windows (PowerShell)**
```bash
python -m venv venv
.\venv\Scripts\Activate.ps1
```

**macOS/Linux**
```bash
python -m venv venv
source venv/bin/activate
```

### 2) Install dependencies
```bash
pip install -r requirements.txt
```

### 3) Run the notebook
Open `week5Lab.ipynb` in VS Code or Jupyter and click **Run All**.

---

## Requirements file
If I change anything in the environment, I regenerate the dependencies using:
```bash
pip freeze > requirements.txt
```

---

## Replicability check (what to do)
To confirm the notebook runs on a clean machine/environment:
1. Create a fresh venv
2. `pip install -r requirements.txt`
3. Run the notebook **top-to-bottom** (Run All)
4. If there are any issues, I note them in the notebook markdown (what failed + how I fixed it)

---

## Talking points (for class)
- I used EDA (shape, missing values, duplicates, summary stats) to understand each dataset before making changes.
- In the Cars section, I handled missing values using both **dropping** and **mean imputation** (and compared before/after).
- In the Diabetes section, I identified outliers using **plots**, **Z-score**, and **IQR**, then removed outliers and compared row counts.
- I kept the notebook steps clear and reproducible (same structure, consistent markdown, and a `requirements.txt`).
- Final step is pushing everything to GitHub with a clean `.gitignore` (no venv tracked).

---

## Git / GitHub (commands I used)
```bash
git init
git add .
git commit -m "Complete Week 5 lab: cleaning, imputation, outlier detection"
git branch -M main
git remote add origin https://github.com/vir33mistry/DataPreProcessingWorkshop.git
git push -u origin main
```

## Author name:
1) Viraj Dipakkumar Mistry, Student ID: 9088985
2) Param Avinashkumar Rasaniya, Student ID: 9086095


