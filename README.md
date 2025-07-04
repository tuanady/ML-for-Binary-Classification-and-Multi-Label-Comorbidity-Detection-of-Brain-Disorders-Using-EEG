# ML-for-Binary-Classification-and-Multi-Label-Comorbidity-Detection-of-Brain-Disorders-Using-EEG
Binary and multi-label classification using CatBoost, SHAP for interpretability, and nested cross-validation. Models generalize well across EEG features and support transparent, reliable decision-making. Designed as a foundation for future clinical tools.

This repository contains results and code for classification experiments involving various disorder pair comparisons and multi-label models. Below is a description of the folder and file structure, along with their contents and purposes.

Folder Structure and Contents
1. Binary Results
    1. all_disorder_pairs_metrics_summary
        Summary metrics for all binary classification disorder pairs. This folder contains performance results such as accuracy, precision, recall, F1-score, and other relevant statistics for each disorder pair tested.

    2. feature_metadata_..._vs_..._fold1...10
        Feature metadata and results for the binary classification task distinguishing across folds 1 to 10 for all disorders. 

    3. fold_metrics_..._vs_... Type
        Fold-wise classification metrics for the binary task differentiating across all pairs. Metrics include fold-wise performance measures such as AUC, accuracy, precision, recall, etc.

    4. metrics_Communication Disorders_vs_Intellectual Disability
        Performance metrics for binary classification comparing across all pairs. This includes aggregated and fold-specific evaluation results.

    5. SHAP Folder 
        Contains SHAP values for all disorder pairs and folds, providing interpretability of feature contributions to model predictions.

2.  Codes
    1. Binary Code
        Scripts and functions for binary classification tasks. Includes data preprocessing, model training, evaluation, metric computation, and visualization tools for disorder pair analyses.

    2. Multi Label Code
        Scripts and utilities for multi-label classification experiments. Supports data preparation, model fitting, multi-label metric calculation, result summarization, and visualizations.

3. Multi Results
    1. model_metrics_...com...
        Evaluation metrics for a multi-class classification model across all subsets and combinations of disorders/classes. Includes accuracy, precision, recall, F1, and other relevant performance measures.

    2. shap_feature_importances_3com1
        SHAP (SHapley Additive exPlanations) feature importance results for the multi-class model, reported across all subsets and class combinations. This provides insight into which features drive model predictions.

    3. subset_average_metrics_summary
        Summary of average performance metrics aggregated over different subsets of data and class combinations for the multi-class model.

4. Usage
    1. Binary Code: Run scripts within this folder to reproduce binary classification experiments. Input data and configuration files should be set accordingly to specify disorder pairs and folds.

    2. Multi Label Code: Use these scripts to run multi-label classification analyses. Make sure to prepare multi-label formatted data and adjust model parameters as needed.

    3. Results Folders: These contain precomputed results that can be used for analysis, visualization, or reporting without rerunning models.

5. Dependencies
    1. This project requires the following Python libraries. You can install them using pip:
            "pip install numpy pandas matplotlib seaborn scikit-learn imbalanced-learn catboost shap chardet xarray"
