# Customer-Segmentation-Practice

## Summary
This project explores two distinct approaches to customer segmentation: 
1. Unsupervised Clustering Methods (including K-Means, Agglomerative Clustering, and DBSCAN, applied to various feature sets derived from customer behavior and demographics to identify natural groupings)
2. Rule-Based-Labels, which define customer segments according to predefined business criteria.

The aim is to systematically compare these two methodologies based on their interpretability, reasonableness, and statistical relevance (evaluated through Chi-square Test, ANOVA, and Mutual Information Score to identify features significantly distinguishing each group). The one that best defines actionable customer groups will be selected and be the target variable for classification models. Model performance will be rigorously assessed using metrics like Precision, Recall, F1-Score, Accuracy, and ROC AUC, guiding the development of personalized and effective marketing strategies.

## Business Context
The "Automobile Retail Customer Segmentation" dataset, available on Kaggle, offers a comprehensive view into customer segmentation tailored for targeted marketing within the automobile retail sector, specifically the bike/ bicycle sector. This dataset is designed to facilitate detailed analyses of customer behaviors and preferences, enabling businesses to identify distinct customer segments and tailor their marketing strategies accordingly.

## Business Goal
The primary goal of this project is to perform customer segmentation and aid the development of related marketing strategies. By analyzing various customer attributes, businesses can gain insights into different customer groups, allowing for more personalized and effective marketing efforts.
The project will begin with unsupervised clustering to identify natural groupings within the customer data. Then, classification models were applied to determine whether these cluster groupings could be effectively predicted based on a subset of significant and correlated features.

## Evaluation Criteria for Data Analysis
To evaluate the effectiveness of the segmentation and subsequent classification, a series of evaluation metrics is adopted. These metrics are used at different stages of the workflow to assess feature significance, clustering relevance, and classification performance:

1.	Chi-square Test

    Used to evaluate the independence between categorical features and cluster labels. A low p-value from Chi-square statistic indicates a strong association, helping to identify features that significantly differ across clusters.

2.	ANOVA (Analysis of Variance)

    Also to test whether there are statistically significant differences in the means of a feature across clusters. The difference with Chi-square is that features applied need to be numerical. A low p-value from ANOVA suggests that the feature varies meaningfully between groups.

3.	Mutual Information Score

    Measures the amount of shared information between a feature and the cluster labels. Higher mutual information indicates a stronger dependency, making the feature more relevant for classification.

4.	Classification Report

    Provides a detailed breakdown of classification performance by presenting several key components for each class. It helps evaluate how well the classification model distinguishes among the clusters.

    (1)	Precision: The ratio of true positives to the sum of true positives and false positives. It measures how accurate the model’s positive predictions are.

    (2)	Recall (Sensitivity): The ratio of true positives to the sum of true positives and false negatives (actual instances of the class that the model failed to identify). It indicates how well the model captures all actual positives.

    (3)	F1-Score: The mean of precision and recall, combining both false positives and false negatives into a single metric to balance the trade-off between them.

    (4)	Support: The total number of actual occurrences of each class in the dataset, showing the true distribution of the classes.

5.	Accuracy Score

    The ratio of the sum of true positives and true negatives to the total number of predictions. It gives a general sense of overall model performance.

6.	ROC AUC Score

    Measures the model’s ability to differentiate between classes. It plots the True Positive Rate against the False Positive Rate at various threshold levels. A higher ROC AUC score reflects better classification performance, especially in imbalanced datasets.

By employing these evaluation metrics, this project aims to ensure both the validity of the unsupervised clustering and the reliability of the following classification models, eventually supporting the goal of deriving actionable insights from customer data for more targeted and effective marketing strategies.
 

