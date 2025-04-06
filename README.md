# Hate_Speech_and_Offensive_Language_Datasez
## Project Description: Hate Speech Detection Using NLP

This project aims to detect **hate speech** and **offensive language** in tweets using advanced Natural Language Processing (NLP) techniques and machine learning models. The dataset, sourced from [Kaggle](https://www.kaggle.com/datasets/thedevastator/hate-speech-and-offensive-language-detection), contains tweets annotated into three categories:

- **0 – Hate Speech**
- **1 – Offensive Language**
- **2 – Neither**

Due to the sensitive nature of the dataset, it includes content that may be racist, sexist, or otherwise offensive, as it reflects real-world behavior and language used on social media.

### Objectives:
- Preprocess and clean raw tweet data (remove duplicates, tokenize, lemmatize)
- Address class imbalance using **SMOTE** oversampling
- Train and evaluate various models including:
  - **SVM (Support Vector Machine)**
  - **Random Forest**
  - **BERT (Transformer-based model)**
- Improve model robustness through hyperparameter tuning and data filtering (e.g., removing low-confidence offensive labels)

## Key Highlights:
- **Data Quality Checks**: No missing values, minimal repetition, outlier detection via tweet length.
- **Preprocessing Pipeline**: Clean text, remove stopwords, lemmatization, and balancing with SMOTE.
- **Imbalance Handling**: The dataset is skewed (~5% hate, ~22% neutral, ~73% offensive). Custom thresholds and sampling strategies were applied.
- **Model Evaluation**: Models are compared on **F1-score**, **ROC AUC**, **accuracy**, and confusion matrices.
- **Iterative Analysis**: Outlier handling, feature selection, and label refinement were used to improve clarity and classification accuracy.

## Conclusion:
Among all models tested, **BERT** achieved the most balanced and accurate performance in detecting hate speech. Its high ROC AUC and F1-score for class 0 make it the most reliable choice for deployment.

