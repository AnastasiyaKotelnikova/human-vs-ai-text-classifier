# Human vs AI Text Classifier

This project focuses on classifying text samples as either **human-written** or **AI-generated** using a custom-built dataset. By combining multiple machine learning models with TF-IDF vectorization, it successfully detects subtle differences in writing styles and structures.

## Key Features

- **Dataset**: 5,000 balanced samples (2,500 human-written and 2,500 AI-generated) — *custom-collected and created by the author for this project*
- **Models Trained**: Logistic Regression, Random Forest, Naive Bayes, Calibrated Linear SVC
- **Text Preprocessing**: Lowercasing, punctuation cleanup, and TF-IDF vectorization
- **Evaluation**: Confusion Matrix, ROC Curve comparisons, Accuracy Scores
- **Visualizations**: Word Clouds, Model Accuracy Bar Charts, ROC Curve Comparisons
- **Output**: Trained model saved to `model/text_classifier_5000.joblib`

## Results

- **Logistic Regression** achieved **100% test accuracy**, followed closely by Calibrated Linear SVC, Naive Bayes, and Random Forest.
- Visual analyses including ROC curves and top predictive words confirmed strong performance.
- The dataset’s clear distinction between classes enabled very high precision without overfitting.

 *Note: The perfect accuracy stems from high separability in the dataset and strong TF-IDF features. This project is meant for educational and experimental purposes.*

---

## Project Structure
```
HUMAN_VS_AI_CUSTOM/
│
├── data/
│   └── your_dataset_5000.csv
│
├── model/
│   ├── model_info.txt
│   └── text_classifier_5000.joblib
│
├── notebooks/
│   ├── Human vs AI Custom Dataset.ipynb
│   └── human_vs_ai_text_classifier.ipynb
│
├── requirements.txt
└── README.md
```

## Author

**Anastasiya Kotelnikova**  
MS Data Science Candidate | NJIT  
Email: [anastasiyakotelnikova21@gmail.com](mailto:anastasiyakotelnikova21@gmail.com)  
[GitHub Profile](https://github.com/AnastasiyaKotelnikova) • [Portfolio Website](https://anastasiyakotelnikova.github.io/Portfolio/) • [LinkedIn](https://www.linkedin.com/in/anastasiyakotelnikova/)
