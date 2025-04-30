Human vs AI Custom Dataset
This project focuses on classifying text samples as either human-written or AI-generated using a custom-built dataset. By combining machine learning models with TF-IDF vectorization, the project successfully detects subtle differences in writing styles and structures.

Key Features
Dataset: 5,000 custom-collected and balanced text samples (Human vs AI).

Models Trained: Logistic Regression, Random Forest, Naive Bayes, and Calibrated Linear SVC.

Text Processing: Lowercasing, punctuation cleanup, and TF-IDF feature extraction.

Evaluation Metrics: Confusion Matrix, ROC Curve Comparisons, and Model Accuracy Scores.

Visualizations: Word Clouds for each class, Accuracy Bar Charts, and ROC Curves for all models.

Results
The Logistic Regression model achieved the highest test accuracy of 100%, followed closely by Linear SVC, Naive Bayes, and Random Forest. Visual analyses such as ROC curves and feature importance further validated the strong model performance. The final trained model has been saved for future deployment.

Note: The 100% test accuracy achieved by the Logistic Regression model is due to the strong separability between human and AI-generated texts in the custom dataset. Text cleaning and TF-IDF vectorization further enhanced feature extraction, enabling the models to perform with very high precision without overfitting.