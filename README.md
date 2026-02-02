# Dagster Reproducible ML Pipeline

## Overview
This project demonstrates a reproducible machine learning pipeline built using Dagster.
It showcases how orchestration improves experiment tracking and execution compared to a non-orchestrated workflow, using the Superstore dataset.
The pipeline covers:
- Data loading
- Data preprocessing
- Exploratory Data Analysis (EDA)
- Model training
- Model evaluation and visualization

## Project Structure
```
dagster-ml-pipeline/
├── data/
│   ├── superstore.csv
│   └── superstore_modified.csv
│
├── python notebook/
│   ├── superstore_dagster.ipynb
│   └── superstore_without_dagster.ipynb
│
├── report/
│   └── With_without_Dagster_time_report.pdf
│
├── pipeline.py
└── README.md
```

## Technologies Used
- Python
- Dagster
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

## Pipeline Description
The Dagster pipeline executes the following steps:
1. Load Dataset - Reads data from the data/ directory.
2. Preprocess Data - Handles missing values, feature selection, and transformations.
3. Exploratory Data Analysis (EDA) - Generates statistical summaries and visualizations.
4. Model Training - Trains multiple machine learning models on the dataset.
5. Model Evaluation - Evaluates performance and visualizes results.
Two dataset variations are supported:
- Original dataset (`superstore.csv`)
- Modified dataset (`superstore_modified.csv`)

## Notebooks
The python notebook/ directory contains:
- `superstore_dagster.ipynb` – ML pipeline implemented using Dagster
- `superstore_without_dagster.ipynb` – ML pipeline without orchestration (baseline comparison)

## How to Run the Dagster Pipeline Locally

### 1. Install dependencies
```bash
pip install dagster dagster-webserver pandas numpy scikit-learn matplotlib seaborn
```

### 2. Start Dagster
```bash
dagster dev -f pipeline.py
```

### 3. Open Dagster UI
Visit:
`http://localhost:3000`

## Report
A comparative performance analysis between Dagster-based and non-Dagster workflows is provided in:
`report/With_without_Dagster_time_report.pdf`

## Results
Execution timelines, model outputs, and performance comparisons are available via:
- Dagster UI
- Included report
