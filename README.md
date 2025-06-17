# 📦 Sentiment-Analysis-on-IMDB-Reviews
Build a text classifier that can detect positive vs negative sentiment from short user reviews

## 🚀 Project Overview
- **Objective:** Classify movie or tweet reviews into positive or negative sentiment
- **Approach:** Preprocess text, extract TF-IDF features (unigram and bigrams) and train a supervised ML model
- **Highlight:** Bigram feature engineering improved F1 score from **89% to 94%**

## 📁 Dataset
- 📂 **Source:** [IMDB Movie Reviews](https://ai.stanford.edu/~amaas/data/sentiment/)  
 _(Alternatively: [Sentiment140 (Twitter)](https://www.kaggle.com/datasets/kazanova/sentiment140))_
- 👥 Binary sentiment: `positive` (1), `negative` (0)
- 🧮 Preprocessed to remove HTML tags, special characters, stopwords, and lowercase everything.


## 🧪 Model Pipeline
| Step | Details |
|------|---------|
| 🔹 Preprocessing | Cleaning, stopword removal, optional lemmatization |
| 🔹 Feature Extraction | `TfidfVectorizer(ngram_range=(1, 2))` |
| 🔹 Model | Logistic Regression |
| 🔹 Evaluation | Accuracy, Precision, Recall, F1-Score, Confusion Matrix |


## 📊 Results
| Metric | Score |
|--------|-------|
| Accuracy | 94.1% |
| Precision | 93.7% |
| Recall | 94.3% |
| F1 Score | 94.0% |

📈 **Improvement:**  
- F1 score increased from **89% → 94%** after switching from unigrams to **bigrams**, which captured key sentiment phrases like `"not good"`, `"very bad"`, and `"absolutely loved"`.
---
## 🧠 Key Learnings
- Bigrams significantly improve sentiment classification by capturing short, meaningful phrases.
- Error analysis helped identify failures with negations and sarcasm.
- Logistic Regression with TF-IDF still performs strongly on clean binary sentiment tasks.
---


**Part of my 20-Day NLP Spring Day#3**