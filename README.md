# Application-3
Comparing Classifiers

# Business Understanding
This project analyzes marketing campaign data from a Portuguese banking institution. The objective was to determine whether a customer would subscribe to a term deposit based on various personal and campaign-related features. To achieve this, we compared the performance of four classification models: K-Nearest Neighbors (KNN), Logistic Regression, Decision Tree, and Support Vector Machine (SVM).

# Model Comparison Summary

1. Logistic Regression: Best Model. It is efficient, accurate and balanced. Best performer with high test accuracy and balanced F1-Score. Precision and recall are reasonable (both classes are performing well). It is fast and reliable. 

2. SVM: Very Strong, but computationally expensive and lower recall. High accuracy, nearly identical to Logistic Regression, but recall is the lowest among all models, which means it's missing more of the minority class. It is the slowest model.

3. KNN: Quick but less robust. With the highest train accuracy after Decision Tree, but generalizes worse. Fast to train. Balanced precision and recall, but not outstanding.

4. Decision Tree: Most overfit. Perfect train accuracy (1.0) but it has the lowest test accuracy, indicating poor generalization. However, F1, precision and recall are all similar, showing consistency in class prediction.

# Recommendations & Next Steps
Keep performing Hyper-parameter tuning
- KNN: Optimize n_neighbors, weights, and distance metric
- Decision Tree: Tune max_depth, min_samples_split, min_samples_leaf
- SVM: Explore different kernels (rbf, poly), C, and gamma
- Logistic Regression: Tune regularization strength (C)

Keep exploring Feature Engineering
- Removing, adding, consolidating features

# Deployment
If Logistic Regression remains the top choice after tuning then we can finalize a scalable preprocessing pipeline, save the model and pipeline and prepare for deployment.
