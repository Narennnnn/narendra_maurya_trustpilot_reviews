# Intent Prediction for Customer Reviews

## Overview

This project aims to predict customer intents or categories from their reviews using Natural Language Processing (NLP) techniques and machine learning. The goal is to automatically classify customer issues or inquiries into predefined categories based on the content of their reviews.

## Approach

### 1. Data Preprocessing

- Review texts are preprocessed to clean and normalize the text:
  - Non-alphabetic characters are removed.
  - Text is converted to lowercase.
  - Tokenization and lemmatization are performed using NLTK (Natural Language Toolkit).
  
### 2. Intent Categorization

- Intents are predefined based on keywords associated with different types of customer issues:
  - **Account -> Lost password**: Keywords include 'password', 'login', 'account'.
  - **Checks -> Mobile deposits -> Void checks**: Keywords include 'check', 'deposit', 'void'.
  - **Debit card -> Declined -> Unauthorized transactions -> fraud**: Keywords include 'unauthorized', 'fraud'.
  - **Invoices -> sent -> unpaid**: Keywords include 'invoice', 'unpaid'.
  - **Invoices -> sent -> paid**: Keywords include 'invoice', 'paid'.
  
### 3. Model Training and Prediction

- A RandomForestClassifier is trained on TF-IDF (Term Frequency-Inverse Document Frequency) vectors of the preprocessed review texts.
- MultiLabelBinarizer is used to handle multiple labels (intents) per review.
- The trained model predicts the intents/categories for new customer reviews.
# narendra_maurya_trustpilot_reviews
![image](https://github.com/Narennnnn/narendra_maurya_trustpilot_reviews/assets/120191897/69a2f232-c4d3-4469-8ca9-163a51dfc604)
