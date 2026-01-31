# Dagster Reproducible ML Pipeline

## Overview
This project demonstrates a reproducible machine learning pipeline using Dagster.
The pipeline performs data loading, preprocessing, EDA, model training, and evaluation
on the Superstore dataset.

## Technologies Used
- Python
- Dagster
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

## Pipeline Description
The pipeline consists of the following steps:
1. Load dataset
2. Preprocess data
3. Perform EDA
4. Train multiple ML models
5. Evaluate and visualize results

Two pipelines are provided:
- Original dataset pipeline
- Modified dataset pipeline

## How to Run (Locally)
```bash
pip install dagster dagster-webserver
dagster dev -f pipeline.py
```
Open http://localhost:3000 in your browser.

## Colab Notebook
The notebook version of this pipeline is available in the `python notebook/` folder.

## Results
Dagster UI screenshots and execution results are available in the `screenshots/` folder.

## Report
The 1-page project report is available in the `report/` folder.
