# NLP Tutorial with NLTK

This repository contains a Jupyter Notebook (`NLP-Tutorial.ipynb`) that walks through core Natural Language Processing (NLP) preprocessing concepts using the NLTK library, including working with corpora, tokenization, n‑grams, frequency distributions, stemming, lemmatization, and stopwords. [attached_file:25]

---

## Contents

The notebook is organized as an end‑to‑end, hands‑on exploration of NLTK:

1. **NLTK Setup and Data Download**
2. **Exploring NLTK Corpora (Movie Reviews, Gutenberg, Hamlet)**
3. **Custom Text Example (AI Paragraph)**
4. **Word and Sentence Tokenization**
5. **Frequency Distribution and Most Common Tokens**
6. **Blankline Tokenization**
7. **Bigrams, Trigrams, and N‑grams**
8. **Stemming (Porter, Lancaster, Snowball)**
9. **Lemmatization (WordNetLemmatizer)**
10. **Stopwords and Basic Cleaning Skeleton** [attached_file:25]

---

## Features Demonstrated

### 1. Environment and NLTK Data Setup

- Downloads essential NLTK resources such as:
  - `punkt` (tokenizer), `stopwords`, `wordnet`, `averaged_perceptron_tagger`, `maxent_ne_chunker`, `words`.
- Optionally downloads the full `popular` NLTK collection.
- Configures a permanent NLTK data path and inspects available corpora. [attached_file:25]

### 2. Working with NLTK Corpora

- Loads and inspects:
  - `movie_reviews` corpus (words).
  - `gutenberg` corpus file IDs.
  - Full word list for *Hamlet* from Shakespeare and prints the first 500 words. [attached_file:25]

This shows how to access and explore built‑in text corpora for experimentation and analysis. [attached_file:25]

### 3. Custom AI Text Example

- Defines a multi‑paragraph string variable containing descriptive text about AI.
- Confirms the data type and uses it as the main sample text for tokenization and further processing. [attached_file:25]

### 4. Tokenization

- Uses `word_tokenize` on the AI text to obtain a list of tokens.
- Computes:
  - Total number of tokens.
  - Word frequency distribution using `FreqDist`.
  - Frequency of specific words (e.g., `"intelligence"`).
  - Top‑10 most common tokens. [attached_file:25]

- Uses `blankline_tokenize` to split the AI text into paragraph‑like chunks and accesses individual segments. [attached_file:25]

### 5. N‑grams (Bigrams, Trigrams, Custom N‑grams)

- Defines a quote string and tokenizes it using NLTK word tokenization.
- Builds and displays:
  - Bigrams: adjacent 2‑word pairs.
  - Trigrams: adjacent 3‑word sequences.
  - 5‑grams using `nltk.ngrams`. [attached_file:25]

This demonstrates how to construct local context windows over tokens, which is useful for language modeling and collocation analysis. [attached_file:25]

### 6. Stemming (Porter, Lancaster, Snowball)

- Initializes three stemmers:
  - `PorterStemmer`
  - `LancasterStemmer`
  - `SnowballStemmer('english')`
- Uses a list like `["give", "giving", "given", "gave"]` and prints each word with its stem under different algorithms to compare how aggressively each stemmer reduces word forms. [attached_file:25]

This section highlights the differences between conservative and aggressive stemming strategies. [attached_file:25]

### 7. Lemmatization (WordNetLemmatizer)

- Initializes a `WordNetLemmatizer`.
- Demonstrates:
  - Lemmatizing plural to singular (e.g., a corpus‑related example).
  - Lemmatizing the same list of words used for stemming to show how lemmatization preserves valid dictionary forms rather than crude stems. [attached_file:25]

This illustrates the contrast between rule‑based stemming and vocabulary‑aware lemmatization. [attached_file:25]

### 8. Stopwords

- Imports English stopwords from `nltk.corpus.stopwords`.
- Prints the English stopword list and checks its length (198 words in the current environment).
- Reuses the earlier frequency distribution for analysis and sets up a regex pattern for punctuation to support further cleaning. [attached_file:25]

This section prepares for classic preprocessing steps such as removing stopwords and punctuation from token lists. [attached_file:25]

---

## File Structure
.
└── NLP-Tutorial.ipynb # Jupyter Notebook containing all code and explanations

The notebook is intended for use in Jupyter Lab / Jupyter Notebook with a Python 3 kernel and NLTK installed. [attached_file:25]

---

## Requirements

To run the notebook:

- Python 3.10+ (the notebook was created with Python 3.12.7)
- Jupyter Notebook or Jupyter Lab
- NLTK

You can install dependencies with:

pip install nltk jupyter

On first run, the notebook will download NLTK corpora and models (may take a few minutes). [attached_file:25]

---

## How to Use

1. Open `NLP-Tutorial.ipynb` in Jupyter.
2. Run the initial cells to download NLTK data and configure the data path.
3. Execute cells sequentially to:
   - Explore corpora.
   - Tokenize custom AI text.
   - Analyze frequency distributions and n‑grams.
   - Compare stemming algorithms.
   - Apply lemmatization.
   - Inspect stopwords and prepare for cleaning. [attached_file:25]

This notebook can serve as both a learning resource and a template for building your own NLP preprocessing pipelines with NLTK. [attached_file:25]

