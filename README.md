# Word Frequency Shift Across Domains

## Overview
This project analyzes how vocabulary usage varies across different domains using the Reuters-21578 dataset. It demonstrates that word frequency distributions are domain-dependent and can be used to understand and classify text.

---

## Objectives
- Analyze word frequency across different domains
- Identify domain-specific vocabulary
- Compare vocabulary distributions across domains
- Demonstrate domain prediction using word patterns
- Handle unknown domains using confidence-based prediction

---

## Dataset
- Dataset: Reuters-21578
- Source: https://kdd.ics.uci.edu/databases/reuters21578/
- Total extracted documents: 8654
- Final filtered documents: 6807

### Selected Domains
- earn (corporate earnings)
- acq (mergers & acquisitions)
- crude (oil market)
- trade (international trade)
- money-fx (foreign exchange)

---

## Methodology

### 1. Data Extraction
- Parsed SGML files using BeautifulSoup
- Extracted article text and topic labels

### 2. Text Preprocessing
- Lowercasing
- Tokenization
- Stopword removal (including custom stopwords)

### 3. Domain-wise Analysis
- Grouped documents by domain
- Computed word frequency for each domain

### 4. Vocabulary Comparison
- Compared top words across domains
- Observed word frequency shifts

### 5. Visualization
- Bar charts for domain-wise top words
- Comparative frequency analysis

---

## Innovation

### 1. Distinctive Word Detection
Identifies words strongly associated with specific domains using relative frequency.

### 2. Explainable Domain Prediction
Predicts the domain of new text and highlights words responsible for the prediction.

### 3. Unknown Domain Detection
Introduces confidence-based classification to avoid incorrect predictions for unseen domains.

---

## Results & Insights
- Each domain exhibits distinct vocabulary patterns
- Financial domains (earn, acq) share similar words
- Crude domain is highly specialized
- Vocabulary distribution varies significantly across domains

---

## Real-World Applications
- News article categorization
- Search engine query understanding
- Email/document classification
- Domain-aware NLP systems

---

## Technologies Used
- Python
- NLTK
- BeautifulSoup
- Pandas
- Matplotlib

---
## Future Improvements
Use TF-IDF for better weighting
Apply machine learning models
Extend to more domains
Improve preprocessing using lemmatization
