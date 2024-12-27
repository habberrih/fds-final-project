# fds-final-project
---
# Sentiment Analysis for the Libyan Misurata Dialect

## Project Overview
This project focuses on developing a sentiment analysis system tailored for the Libyan Misurata dialect, an underrepresented Arabic dialect. Using customized preprocessing techniques, including stemming, lemmatization, and a dialect-specific stopword list, the system achieves improved performance on sentiment classification tasks. The project evaluates the effectiveness of machine learning classifiers such as Logistic Regression, Naive Bayes, and SVM with various preprocessing strategies.

## Preprocessing Techniques
The preprocessing phase involves the following techniques:
- **Standard Arabic Character Normalization**: Normalizes characters like "أ", "إ", and "آ" to "ا".
- **Diacritics Removal**: Removes diacritics to simplify the text.
- **Stopword Removal**: Removes a custom list of stopwords specific to the Libyan dialect.
- **Stemming and Lemmatization**: Extracts root forms of words using a customized Libyan analyzer.

## Classifiers and Evaluation
The classifiers used include:
- **Logistic Regression**
- **Naive Bayes**
- **SVM (Support Vector Machine)**

### Results
The results highlight the impact of various preprocessing strategies on sentiment classification accuracy. The table below summarizes the accuracy for different experiments:

| Experiment                                | Logistic Regression | Naive Bayes | SVM   |
|-------------------------------------------|----------------------|-------------|-------|
| Lemmatization with Stopword Removal       | 0.72                | 0.68        | 0.74  |
| Lemmatization without Stopword Removal    | 0.70                | 0.65        | 0.71  |
| Stemming with Stopword Removal            | 0.73                | 0.69        | 0.75  |
| Stemming without Stopword Removal         | 0.71                | 0.67        | 0.72  |
| Stemming and Lemmatization with Stopwords | 0.74                | 0.70        | 0.76  |
| Stemming and Lemmatization without Stopwords | 0.72             | 0.66        | 0.73  |

The chart below visualizes these results:

![Classifier Accuracy with Optimized N-grams](./results.png)

## Usage

### Preprocessing
The customized Libyan dialect analyzer performs:
1. Tokenization.
2. Standard Arabic character normalization.
3. Stopword removal.
4. Stemming and lemmatization.


## Conclusion
This project demonstrates that combining preprocessing techniques, including stemming, lemmatization, and stopword removal, improves sentiment analysis performance in the Libyan Misurata dialect. The customized preprocessing pipeline and SVM classifier yielded the best results.

![results](https://github.com/user-attachments/assets/87fa74f8-e84e-4799-8feb-3833eec9a72f)
