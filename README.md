# Machine Learning Sports Injury Analysis

> Machine learning pipeline for predicting sports injury risk from multimodal physiological and biomechanical data.

![Python](https://img.shields.io/badge/Python-3.x-blue)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange)
![License](https://img.shields.io/badge/License-MIT-green)

## 📊 Overview

Sports injuries can significantly impact athletes' performance and career longevity. Being able to identify individuals at elevated injury risk before an injury occurs enables coaches and medical staff to optimize training loads and implement preventive interventions.

This project develops a machine learning workflow to predict injury risk using physiological, biomechanical and training-related variables. The repository covers every stage of the analysis, from raw data preprocessing to model interpretation.

The entire workflow is implemented in a single Jupyter notebook.

## ⭐ Objectives

The project aims to:

- Build a complete machine learning pipeline for injury risk prediction.
- Explore relationships between physiological variables and injury occurrence.
- Compare injury risk classes through exploratory data analysis.
- Train and optimize a Random Forest classifier.
- Interpret model predictions using feature importance analysis.

## ​📃​ Dataset

The project uses the **Multimodal Sports Injury Dataset**, publicly available on Kaggle.

The notebook automatically downloads the dataset using `kagglehub`.

## ​🏛️​ Repository Structure

```
Machine-Learning-Sports-Injury-Analysis/
│
├── analysis.ipynb        
├── dataset.csv
└── README.md
```

## 🚀 Important ML features

Recursive Feature Elimination (RFE) is applied using a Random Forest estimator to identify the most informative predictors.

A Grid Search is performed to optimize Random Forest hyperparameters.

Performance is evaluated through several metrics (precision & recall, F1-score, confusion matrix):

## ​💎​​ Key Findings

The analysis revealed that:

- Several physiological variables strongly contribute to injury prediction.
- Healthy and Low Risk athletes exhibit substantial overlap in feature space.
- Merging Healthy and Low Risk into a single class substantially improves classification performance.


## ​💿​ Installation

Clone the repository:

```bash
git clone https://github.com/victor-fdz/Machine-Learning-Sports-Injury-Analysis.git
cd Machine-Learning-Sports-Injury-Analysis
```

Install the required packages:

```bash
pip install pandas numpy matplotlib seaborn scipy scikit-learn imbalanced-learn kagglehub
```

## 💻​ Usage

Launch the notebook:

```bash
jupyter notebook sports_injury_analysis.ipynb
```

Run all cells sequentially to reproduce the complete analysis.

## ​🙋‍♂️​ Author

**Víctor Fernández Oliveras**
https://www.linkedin.com/in/victor-fdz/


This repository is released under the MIT License.
