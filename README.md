# Human vs AI Text Classifier

This project focuses on classifying text samples as either **human-written** or **AI-generated** using a custom-built dataset. By combining multiple machine learning models with TF-IDF vectorization, it successfully detects subtle differences in writing styles and structures.

## Key Features

- **Dataset**: 5,000 balanced samples (2,500 human-written and 2,500 AI-generated) — *custom-collected and created by the author for this project*
- **Models Trained**: Logistic Regression, Random Forest, Naive Bayes, Calibrated Linear SVC
- **Text Preprocessing**: Lowercasing, punctuation cleanup, and TF-IDF vectorization
- **Evaluation Metrics**: Confusion Matrices, ROC Curves, AUC Scores, Classification Reports
- **Visualizations**: Word Clouds, Model Accuracy Bar Charts, ROC Curve Comparisons, Feature Importance
- **Output**: Saved model with `joblib` in `/model/text_classifier_5000.joblib`

## Results

- **Logistic Regression** achieved **100% test accuracy**, followed closely by Calibrated Linear SVC (0.998), Naive Bayes (0.997), and Random Forest (0.992).
- **Feature Importance**: TF-IDF weights revealed words most indicative of AI vs. human writing.
- **ROC Curves & AUC Scores** validated model separability and classification power.
- **Classification Reports** confirmed high precision, recall, and F1-scores across all models.

 *Note: Perfect accuracy reflects the high separability of the dataset and strong TF-IDF features. The project is designed for educational and experimental exploration._

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
