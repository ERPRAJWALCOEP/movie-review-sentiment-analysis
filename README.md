# 🎬 Movie Review Sentiment Analysis using NLP

A Machine Learning project that classifies movie reviews as positive or negative using Natural Language Processing techniques.

---

## 📌 Project Overview

This project develops a Sentiment Analysis Tool for movie reviews.

The system preprocesses review text, extracts TF-IDF features and compares multiple machine learning algorithms. The model with the best F1-score is selected and saved for future predictions.

The project matches the Codec Technologies internship topic:

> Sentiment Analysis Tool – Develop a model to analyze sentiments in text data, such as movie reviews.

---

## 📂 Dataset

The project uses the NLTK Movie Reviews dataset.

- Total reviews: **2,000**
- Positive reviews: **1,000**
- Negative reviews: **1,000**
- Training samples: **1,600**
- Testing samples: **400**
- Classes: Positive and Negative

---

## 🧹 Text Preprocessing

The preprocessing pipeline includes:

- Converting text to lowercase
- Removing URLs
- Removing HTML tags
- Removing punctuation
- Removing numbers
- Removing extra spaces
- Removing English stop words
- Lemmatizing words
- Removing very short tokens

---

## 🔤 Feature Extraction

The cleaned movie reviews are converted into numerical features using:

- TF-IDF Vectorization
- Unigrams and bigrams
- Maximum 20,000 features
- Minimum document frequency of 2

---

## 🧠 Models Compared

Three supervised machine learning models were trained and evaluated:

1. Logistic Regression
2. Multinomial Naive Bayes
3. Linear Support Vector Machine

---

## 📊 Model Performance

| Model | Accuracy | Precision | Recall | F1-score |
|---|---:|---:|---:|---:|
| Logistic Regression | 83.00% | 81.73% | 85.00% | 83.33% |
| Multinomial Naive Bayes | 81.75% | 80.68% | 83.50% | 82.06% |
| **Linear SVM** | **84.50%** | **82.24%** | **88.00%** | **85.02%** |

### Best Model

**Linear SVM** was selected because it achieved the highest F1-score.

---

## 📈 Confusion Matrix Results

The Linear SVM model produced:

- True Negatives: **162**
- False Positives: **38**
- False Negatives: **24**
- True Positives: **176**

The model correctly classified:

```text
338 out of 400 test reviews
```

---

## 🖼️ Project Screenshots

### Dataset

![Dataset](images/dataset.png)

### Preprocessing

![Preprocessing](images/preprocessing.png)

### Model Results

![Model Results](images/model_results.png)

### Model Comparison

![Model Comparison](images/model_comparison.png)

### Classification Report

![Classification Report](images/classification_report.png)

### Confusion Matrix

![Confusion Matrix](images/confusion_matrix.png)

### Sample Predictions

![Sample Predictions](images/sample_predictions.png)

### Model Saved

![Model Saved](images/model_saved.png)

---

## 🛠️ Technologies Used

- Python
- NLTK
- Pandas
- NumPy
- Scikit-learn
- TF-IDF
- Logistic Regression
- Multinomial Naive Bayes
- Linear SVM
- Matplotlib
- Seaborn
- Joblib
- Google Colab

---

## ▶️ How to Run

1. Download or clone this repository.
2. Open `Movie_Review_Sentiment_Analysis.ipynb` in Google Colab or Jupyter Notebook.
3. Install the required libraries:

```bash
pip install -r requirements.txt
```

4. Run all notebook cells in sequence.
5. Review the model comparison and evaluation results.
6. Use the custom prediction function to classify new movie reviews.

---

## 💡 Sample Predictions

```text
Review:
The movie was excellent, emotional and beautifully acted.

Prediction:
Positive
```

```text
Review:
This was a boring film with a weak story and terrible acting.

Prediction:
Negative
```

---

## 💾 Saved Model

The best-performing pipeline is saved as:

```text
movie_review_sentiment_model.joblib
```

This saved pipeline includes:

- TF-IDF Vectorizer
- Linear SVM classifier

---

## 🚀 Future Improvements

- Use a larger IMDb movie-review dataset
- Add neutral-sentiment classification
- Use word embeddings such as Word2Vec or GloVe
- Compare performance with LSTM, BERT or RoBERTa
- Build a Streamlit web application
- Deploy the model as an API

---

## 👨‍💻 Author

**Prajwal Sonawane**

M.Tech – AI in Signal Processing  
COEP Technological University, Pune
