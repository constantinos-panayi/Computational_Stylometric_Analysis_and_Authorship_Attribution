# Computational Stylometric Analysis and Authorship Attribution

### An Exploratory Comparative Study of the Literary Styles of Mark Twain and Charles Dickens

## Overview

This repository presents an **exploratory computational stylometric analysis** of twenty literary works authored by **Mark Twain** and **Charles Dickens**.

Situated within a **Digital Humanities** framework, the project combines **Natural Language Processing (NLP)**, **stylometric feature extraction**, **statistical analysis**, and **Machine Learning** techniques to investigate whether quantifiable linguistic patterns can effectively distinguish between the writing styles of the two authors.

The study examines literary style through multiple analytical dimensions, including lexical diversity, syntactic structure, grammatical composition, and affective expression.

This project constitutes the **final project for the Data Analysis for Humanities with Python course** of the **MSc Digital Humanities programme**, jointly offered by the National and Kapodistrian University of Athens, the University of Cyprus, and the ATHENA Research Centre.

---

## Research Objectives

The project addresses the following research questions:

* Are there measurable lexical differences between the works of Mark Twain and Charles Dickens?
* Are there measurable syntactic differences between their writing styles?
* Do the authors exhibit distinct grammatical patterns?
* Are there detectable differences in the affective characteristics of their texts?
* Do stylometric features produce meaningful author-based clusters?
* Can Machine Learning methods accurately classify texts according to their author?

---

## Dataset Description

The corpus consists of **20 literary works**, equally divided between the two authors.

All texts were collected from **Project Gutenberg** and processed through a Natural Language Processing pipeline designed for stylometric analysis.

---

## Methodology

### Data Preprocessing

Three complementary corpus representations were constructed:

* Raw Corpus
* Sentence Corpus
* Cleaned Corpus

Preprocessing procedures included:

* Lowercasing
* Punctuation removal
* Stopword removal
* Tokenisation

Lemmatisation was intentionally omitted in order to preserve stylistically meaningful lexical variation.

---

### Stylometric Feature Extraction

A total of **14 stylometric features** were extracted across four analytical dimensions.

#### Lexical Features

* Type-Token Ratio (TTR)
* Measure of Textual Lexical Diversity (MTLD)
* Hypergeometric Distribution Diversity (HD-D)

#### Syntactic Features

* Average Sentence Length (ASL)
* Passive Voice Rate (PVR)

#### Grammatical Features

* Noun percentage
* Verb percentage
* Adjective percentage
* Adverb percentage
* Pronoun percentage

#### Affective Features

Using the VADER sentiment analysis framework:

* Negative sentiment
* Neutral sentiment
* Positive sentiment
* Compound sentiment

---

## Statistical Analysis and Modelling

### Correlation Analysis

* Pearson Correlation Matrix
* Feature relationship exploration
* Multicollinearity assessment

### Principal Component Analysis (PCA)

* Dimensionality reduction
* Explained Variance Ratio (EVR)
* Principal Component Loadings
* Author-based clustering analysis

### Machine Learning Classification

#### Binomial Logistic Regression

* Authorship attribution
* Feature importance evaluation

#### Model Validation

* Stratified 5-Fold Cross Validation
* Confusion Matrix
* Performance Metrics
* ROC Curve
* Area Under the Curve (AUC)

---

## Key Findings

### Lexical Style

* Mark Twain exhibits higher lexical diversity and greater stylistic variation.
* Charles Dickens demonstrates a more consistent lexical profile across works.

### Syntactic Style

* Dickens tends to employ longer sentences and a slightly higher passive voice rate.
* Twain exhibits greater variability in syntactic structure.

### Grammatical Style

* Grammatical distributions are broadly similar across both authors.
* POS features provide limited discriminatory power.

### Affective Style

* Dickens exhibits higher compound sentiment scores and a more positive emotional orientation.
* Twain displays a more neutral affective profile.

### Principal Components

* The first three principal components explain approximately 73.5% of total variance.
* PCA reveals meaningful author-related stylistic separation.

### Authorship Attribution

* Logistic Regression achieved:

  * Accuracy: 80%
  * Precision: 80%
  * Recall: 80%
  * F1-score: 80%
  * AUC: 0.85

These results demonstrate that stylometric features contain sufficient information to support automated authorship attribution.

---

## Repository Structure

├── CODE_Computational_Stylometric_Analysis.ipynb

├── REPORT_Computational_Stylometric_Analysis.pdf

├── README.md

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* NLTK
* LexicalRichness
* Scikit-learn
* VADER Sentiment Analysis

---

## License

**Academic Use – Coursework License**

This repository contains coursework developed within the MSc Digital Humanities programme.

The material is intended exclusively for academic, educational, and research purposes. Commercial use, redistribution, or modification without explicit permission from the author is prohibited.

---

## Author

**Constantinos Panayi**

Postgraduate Student, MSc Digital Humanities

National and Kapodistrian University of Athens • University of Cyprus • ATHENA Research Centre
