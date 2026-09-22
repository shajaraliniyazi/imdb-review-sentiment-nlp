# IMDB Review Sentiment — NLP Preprocessing & EDA

An end-to-end text preprocessing and exploratory data analysis pipeline for the [IMDB 50K Movie Reviews](https://ai.stanford.edu/~amaas/data/sentiment/) dataset, built to prepare raw movie reviews for sentiment classification.

## What's inside

- **`text based project.ipynb`** — the full pipeline, from raw text to analysis-ready data:
  - Duplicate removal and lowercasing
  - HTML tag stripping, punctuation/number cleanup with regex
  - Contraction expansion (`don't` → `do not`, etc.)
  - Tokenization with NLTK, sentiment-aware stopword removal (negations like *not*, *no*, *never* are kept)
  - Exploratory analysis: sentiment balance, review length distributions, most frequent words and bigrams, word clouds, and positive vs. negative comparisons
- **`IMDB Dataset.csv`** — the raw dataset: 50,000 movie reviews labeled `positive` or `negative`.

## Tech stack

`pandas` · `nltk` · `scikit-learn` · `matplotlib` · `seaborn` · `wordcloud`

## Getting started

```bash
pip install pandas nltk scikit-learn matplotlib seaborn wordcloud
```

Open `text based project.ipynb` in Jupyter and run the cells top to bottom. NLTK resources (`punkt_tab`, `stopwords`) are downloaded automatically on first run.

## Dataset

50,000 reviews, roughly balanced between positive and negative sentiment, sourced from the classic IMDB sentiment analysis dataset.
