# Machine-Learning-Sports-Injury-Analysis
This project utilizes a Random Forest pipeline to classify athlete injury risk into three categories: Healthy, Low Risk, and High Risk/Injured. 

# 📊 Methodology & Workflow
## Data Preprocessing
- Cleaning: due to MCAR and high data volume, NAs were deleted.
- Violin + Boxplot + Histogram: multimodal plot to capture statistical information.

## Model Interpretation
- Feature importance: ranking of variables (with previous feature selection with RFE)
- Confusion matrices.
- Feature distribution overlapping: detected by KDE plots and PCA, explains the model's constrains.  

# 🚀 Key Results
- Clear separation of High risk/Injured profiles.
- Identified top predictors of injuries.
- Systemic recovery is a more critical predictor than biomechanical markers.


### Specifications: 
Python 3.13.5
