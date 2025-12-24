# quora-question-pairs
A NLP project to find weather given 2 questions are same are not semantically speaking.

🔹 Project Summary

Built an end-to-end NLP feature engineering pipeline for detecting duplicate question pairs using EDA, text preprocessing, handcrafted linguistic features, and Bag of Words (BoW).

The project demonstrates strong fundamentals in data analysis, NLP preprocessing, and feature engineering, commonly used in real-world ML systems.

🔹 Problem Statement

Given two questions, determine whether they convey the same intent.

🔹 Dataset

Question pair dataset (question1, question2)

Binary target: is_duplicate

Sampled 60,000 records for efficient experimentation

🔹 Exploratory Data Analysis (EDA)

Performed EDA to understand data quality and structure:

Class distribution (duplicate vs non-duplicate)

Missing and empty questions

Question length and word count analysis

Comparison of text characteristics across classes

📌 Key Insight:
Duplicate questions tend to have similar lengths and higher word overlap, motivating similarity-based feature engineering.

🔹 Text Preprocessing

Implemented a custom preprocessing pipeline:

Lowercasing

HTML removal

Punctuation and special character removal

Contraction expansion

Whitespace normalization

Ensures clean and consistent textual input for modeling.

🔹 Feature Engineering
Basic Features

Character length of questions

Word count per question

Advanced Linguistic Features

Common word count

Unique word count

Word overlap ratio

Absolute and mean word count difference

Token-level similarity metrics

Bag of Words (BoW)

Used CountVectorizer to convert text into numerical vectors

Generated BoW features for both questions

Combined BoW vectors with handcrafted numerical features

🔹 Skills Demonstrated

Exploratory Data Analysis (EDA)

NLP preprocessing

Feature engineering for text similarity

Bag of Words modeling

Data cleaning and transformation

Python (Pandas, NumPy, Scikit-learn)

🔹 Tools & Libraries

Python

Pandas, NumPy

Scikit-learn

Regular Expressions

BeautifulSoup

Matplotlib / Seaborn

🔹 Project Workflow

Data loading and sampling

Exploratory Data Analysis

Text preprocessing

Feature engineering (basic + advanced)

Bag of Words vectorization

Final feature matrix preparation

🔹 Future Enhancements

Replace BoW with TF-IDF

Use word embeddings (Word2Vec / GloVe)

Train ML models (Logistic Regression, XGBoost)

Handle class imbalance

Extend to transformer-based models

🔹 Why This Project Matters

This project reflects industry-relevant NLP practices, focusing on clean data, meaningful features, and explainable modeling foundations, which are critical before applying complex ML or deep learning models.

Dataset Link - https://www.kaggle.com/c/quora-question-pairs
