# Credit Risk Analysis

## Overview
The purpose of the analysis is to train and test the credit card credit dataset through various evaluation models to determine which model should be used to predict credit risk.

## Results
* Random Oversampling<br>
    - Balanced Accuracy Report<br>
    ![Random Oversampling Accuracy](Resources/ros_report.jpg) <br>
    - Precision & Recall Report <br>
    ![Random Oversampling Precision and Recall](Resources/ros_classification.jpg)<br><br>
* SMOTE<br>
    - Balanced Accuracy Report<br>
    ![SMOTE Accuracy](Resources/smote_report.jpg)<br>
    - Precision & Recall Report <br>
    ![SMOTE Precision and Recall](Resources/smote_classification.jpg)<br><br>
* Cluster Centroids<br>
    - Balanced Accuray Report<br>
    ![Cluster Centroids Accuracy](Resources/cc_report.jpg)<br>
    - Precision & Recall Report <br>
    ![Cluster Centroids Precision and Recall](Resources/cc_classification.jpg)<br><br>
* SMOTEENN<br>
    - Balanced Accuray Report<br>
    ![SMOTEENN Accuracy](Resources/enn_report.jpg)<br>
    - Precision & Recall Report <br>
    ![SMOTEENN Precision and Recall](Resources/enn_classification.jpg)<br><br>
* Random Forest<br>
    - Balanced Accuray Report<br>
    ![Random Forest Accuracy](Resources/rf_report.jpg)<br>
    - Precision & Recall Report - highest precision & recall rate<br>
    ![Random Forest Precision and Recall](Resources/rf_classification.jpg)<br><br>
* Easy Ensemble<br>
    - Balanced Accuray Report - highest accuracy rate<br>
    ![Easy Ensemble Accuracy](Resources/eec_report.jpg)<br>
    - Precision & Recall Report <br>
    ![Easy Ensemble Precision and Recall](Resources/eec_classification.jpg)<br>

## Summary

Throughout different testing models, "Easy Ensemble" had the highest balanced accuracy (0.926) while "Random Forest" showed the highest precicion & recall rates (see below image). <br>
    ![Random Forest Precision and Recall](Resources/rf_classification.jpg)<br><br>

Credit reporting requires high rates all categories of accuracym, precision, and recall. However, none of the models have resulted with high rates in all 3 categories. Although random forest model showed highest precision & recall rates amongst all the models, the recall rate for high risk is only at 0.32, meaning only 32% of the high risk credit will be diagnosed as high risk. In easy ensemble model, the recall rates on both the high risk and low risk were over 90%; however, precision rate on high risk was only at 8%, which means there could be a lot of false-reportings for high risk credit reports. Therefore, none of the models will fit to analyze the credit card credit data.