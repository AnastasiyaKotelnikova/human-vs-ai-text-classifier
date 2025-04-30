# Human vs AI Text Classifier

This project builds a binary text classification system to distinguish between **human-written** and **AI-generated** text using a custom-labeled dataset. By combining **TF-IDF vectorization** with multiple machine learning models, it captures subtle linguistic patterns and style differences across writing sources.

---

## Key Highlights

- **Custom Dataset**: 5,000 samples (2,500 human + 2,500 AI-generated), curated and balanced by the author.
- **Models Trained**:
  - Logistic Regression (Top performer: **100% accuracy**)
  - Random Forest
  - Multinomial Naive Bayes
  - Calibrated Linear SVC
- **Text Preprocessing**:
  - Lowercasing
  - Punctuation removal
  - Token cleaning
- **Evaluation Metrics**:
  - Confusion Matrices
  - ROC Curves & AUC Scores
  - Precision, Recall, F1-Score
- **Visual Interpretations**:
  - Word Clouds
  - Feature Importance Bar Charts
  - Model Accuracy Comparison
- **Deployment Ready**:
  - Final model serialized with `joblib`
  - Predicts new input instantly

---

## Results Summary

| Model               | Accuracy | AUC Score |
|--------------------|----------|-----------|
| Logistic Regression| **1.000**| 1.00      |
| Linear SVC         | 0.998    | -         |
| Naive Bayes        | 0.997    | 1.00      |
| Random Forest      | 0.992    | 1.00      |

- **TF-IDF feature weights** revealed strong interpretability.
- **Words like “industry”, “AI”, “intelligence”** were predictive of AI text.
- **Words like “my”, “was”, “weather”** were highly human-like.
- ROC curves confirmed excellent model separability.

> *Note: Perfect accuracy is expected due to the high separability and structured nature of the dataset (intended for educational use).*

---

## Project Structure

```
HUMAN_VS_AI_CUSTOM/
├── data/
│   └── your_dataset_5000.csv             # Final cleaned and labeled dataset (2,500 Human + 2,500 AI samples)
├── model/
│   ├── model_info.txt                    # Description of model version and training details
│   └── text_classifier_5000.joblib       # Serialized trained model for deployment
├── notebooks/
│   ├── Human vs AI Custom Dataset.ipynb  # Main notebook with training, evaluation, and analysis
│   └── human_vs_ai_text_classifier.ipynb # Optional/experimental version or backup notebook
├── requirements.txt                      # Python libraries used in the project
└── README.md                             # Project overview and instructions
```
