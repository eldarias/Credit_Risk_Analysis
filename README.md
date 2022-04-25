# Credit_Risk_Analysis
Module 17: Supervised Machine Learning and Credit Risk

---
## Overview
The purpose of this challenge is to use Machine Learning to analyze the dataset from **LendingClub**.  The dataset is unbalanced where good loans outnumber risky loans therefore different techniques learned throughout the module need to be implemented to train and evaluate models with unbalanced classes.

The challenge consists of the following 4 Deliverables:
- Deliverable 1: Use Resampling Models to Predict Credit Risk
- Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk
- Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
- Deliverable 4: A Written Report on the Credit Risk Analysis (README.md)

---

## Results:
Below are the results from each deliverable:
- **Deliverable 1:** Use Resampling Models to Predict Credit Risk (Three Machine Learning Models used; RandomOverSampler, SMOTE, & ClusterCentroids)
    - <image src="./Results/Deliverable1_RandomOverSample_Results.PNG"></p>
        - balanced accuracy score = 0.6573009382322703 (see output above)
        - confusion matrix results: 72 = TP, 29 = FN, 6,812 = FP, 10,292 = TN (see output above)
        - imbalanced classification report = (see output above)
    - <image src="./Results/Deliverable1_SMOTE_Oversampling_Results.PNG"></p>
        - balanced accuracy score = 0.6622479600626106 (see output above)
        - confusion matrix results: 64 = TP, 37 = FN, 5,288 = FP, 11,816 = TN (see output above)
        - imbalanced classification report = (see output above)
    - <image src="./Results/Deliverable1_ClusterCentroids_Undersampling_Results.PNG"></p>
        - balanced accuracy score = 0.5447339051023905 (see output above)
        - confusion matrix results: 70 = TP, 31 = FN, 10,324 = FP, 6,780 = TN (see output above)
        - imbalanced classification report = (see output above)

- **Deliverable 2:** Use the SMOTEENN Algorithm to Predict Credit Risk
    - <image src="./Results/Deliverable2_SMOTEENN_Under-and-Over-Sampling_Results.PNG"></p>
    - This deliverable combines over and under sampling algorithm (SMOTEENN) to determine if the results perform better than the previous samplings.
        - balanced accuracy score = 0.644711676499736 (see output above)
        - confusion matrix results: 73 = TP, 28 = FN, 7,412 = FP, 9,692 = TN (see output above)
        - imbalanced classification report = (see output above)

- **Deliverable 3:** Use Ensemble Classifiers to Predict Credit Risk
    - <image src="./Results/Deliverable3_EE-AdaBoost_Results.PNG"></p>
        - balanced accuracy score = 0.9316600714093861 (see output above)
        - confusion matrix results: 93 = TP, 8 = FN, 983 = FP, 16,121 = TN (see output above)
        - imbalanced classification report = (see output above)

---

## Summary:
In summary, the best results were observed by Easy Ensembled AdaBoost.  For high-risk loans predictions, the analysis reported a balanced accuracy score of .93, a precision score of 0.09, a recall score of 0.92 and a F1 score of 0.16.  This Machine Learning algorithm can be used to make future predictions, but it is important to note that the dataset is unbalanced where high-risk loans is the minority.