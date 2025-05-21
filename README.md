# Evaluating-IBD-Flares-Predictors

This repository contains the code and documentation for all statistical analyses performed in the study. The analysis was conducted using a Group Lasso (G-Lasso) modeling approach to identify key predictors of interest. Six G-Lasso models were built, with feature selection guided by clinical relevance and domain knowledge. A nested cross-validation framework (Stratified Hold-Out + Inner Cross Validation) was implemented to optimize hyperparameters (λ) and ensure robust model generalizability.

Model performance was evaluated on an untouched test set (30%) using metrics such as AUC (Area Under the Curve) , with confidence intervals reported for transparency. Significant predictors were identified by extracting non-zero coefficients from the optimal models. Statistical comparisons between models were performed using either Repeated Measures ANOVA or the Friedman test , depending on normality assumptions, with post-hoc pairwise comparisons to assess differences.

All scripts are well-documented and include steps for data preprocessing, model training, validation, and performance evaluation. Dependencies and instructions for replication are provided in the respective files.
