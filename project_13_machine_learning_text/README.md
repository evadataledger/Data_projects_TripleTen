# Project 13: Machine Learning for Text – Movie Review Sentiment Classifier

## Objective
Train a classification model to detect **negative movie reviews** from IMDb using machine learning.  
Achieve an **F1 score of at least 0.85** on the test set.

---

## Dataset
- `imdb_reviews.tsv`
- Columns:
  - `review`: full user review
  - `pos`: target label (1 = positive, 0 = negative)
  - `ds_part`: train or test partition

---

## Techniques Used
- Text preprocessing (tokenization, lemmatization, lowercasing)
- Feature extraction using **TF-IDF**
- Classifier comparison:
  - Logistic Regression
  - Gradient Boosting
  - (Bonus) BERT via Transformers
- Evaluation Metrics:
  - F1 Score
  - Confusion Matrix
  - ROC-AUC

---

## Libraries & Tools
- `pandas`, `numpy`
- `nltk`
- `scikit-learn`
- `transformers`, `torch`
- `matplotlib`, `seaborn`

---

## Results
- Final F1 Score: **≥ 0.85**
- Stronger performance with Logistic Regression + TF-IDF
- BERT provided improvement but requires more compute

---

## What I Learned
- Real-world text classification pipeline
- Importance of feature extraction in NLP
- Model comparison and trade-offs in NLP workflows

---

## Note
Due to dataset size, data not included. See `/data/README.md` for more info.

## Folder Structure

```bash
project_13_machine_learning_text/
├── notebooks/
│   └── project_13_movie_review_sentiment.ipynb
├── data/
│   └── README.md (dataset not included)
├── requirements.txt
└── README.md
