# Machine-Learning-Sports-Injury-Analysis
Predicting Sports Injury Risk: A Machine Learning Analysis of Integrated Physiological and Biomechanical Data. Work for HPC and Big Data Analysis of my MSc in Bioinformatics

Athlete Injury Risk Assessment: Biomechanical Multi-Class Classification
This project implements a machine learning pipeline to predict injury risk in athletes based on biomechanical, physiological, and workload data. Originally designed as a binary classifier, the project evolved into a three-class model to better distinguish between Healthy, Low Risk, and High Risk categories.

📋 Project Overview
The goal is to move beyond simple "injured vs. non-injured" binary labels to provide a more nuanced risk profile. This allows for proactive intervention strategies in sports performance environments.

Key Features:
Multi-Class Classification: Random Forest and Gradient Boosting models optimized for categorical risk.

Advanced Visualization: Distribution analysis using a "Violin + Boxplot + Histogram" trio for feature characterization.

Dimensionality Reduction: PCA analysis to visualize class separation and variance.

Statistical Analysis: Correlation matrices and Gini feature importance ranking.

🛠️ Tech Stack
Language: Python

Data Science: pandas, numpy, scikit-learn

Visualization: matplotlib, seaborn

Formats: All plots are exported in SVG (Scalable Vector Graphics) for high-resolution publication quality.

📊 Visualizations & Methodology
1. Feature Distribution Analysis
We analyze predictor variables using a dual-plot approach:

Left: Violin plots with integrated boxplots to show density and quartiles.

Right: Horizontal histograms to show absolute frequency.

Colors: Utilizes the viridis colormap with standardized alpha transparency (0.5 - 0.6) for clarity.

2. Feature Importance & KDEs
We extract the top predictor variables (e.g., recovery_score, fatigue_index) and analyze their overlap across classes using Kernel Density Estimate (KDE) plots.

Customization: Titles are figure-centered (not axes-centered) with common Y-axis labels for a clean, academic look.

3. Confusion Matrix
A normalized confusion matrix provides insight into model performance, specifically highlighting the "confusion" between Healthy and Low Risk classes.

🚀 How to Run
Clone the repo:

Bash

git clone https://github.com/your-username/injury-risk-classification.git
Install dependencies:

Bash

pip install -r requirements.txt
Execute the notebook:
Open analysis.ipynb to view the data cleaning, training, and SVG generation logic.

📈 Results Summary
Top Predictors: The model identified that workload balance and recovery scores are the primary drivers of risk.

PCA Performance: Two principal components explain approximately X% (update with your value) of the variance, showing distinct clustering for High-Risk athletes.
