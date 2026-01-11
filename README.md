# Quora Question Pairs – Duplicate Question Detection

An **NLP-based project** to determine whether two questions are **semantically equivalent**, even if they are phrased differently.  
The project focuses on **EDA, text preprocessing, and feature engineering**, forming a strong foundation for real-world machine learning systems.

---

## 📌 Project Summary

This project builds an **end-to-end NLP feature engineering pipeline** for detecting duplicate question pairs. It emphasizes:

- Exploratory Data Analysis (EDA)
- Text preprocessing
- Handcrafted linguistic feature engineering
- Bag of Words (BoW) representation

The goal is to demonstrate **core NLP and data analysis skills** before applying advanced ML or deep learning models.

---

## ❓ Problem Statement

Given two questions, determine whether they **convey the same intent**.

---

## 📂 Dataset

- **Source:** Quora Question Pairs Dataset
- **Features:**
  - `question1`
  - `question2`
- **Target Variable:**
  - `is_duplicate` (binary classification)
- **Sampling:**
  - Used **60,000 records** for efficient experimentation

🔗 **Dataset Link:**  
https://www.kaggle.com/c/quora-question-pairs

---

## 🔍 Exploratory Data Analysis (EDA)

Performed EDA to understand dataset structure and quality:

- Class distribution (duplicate vs non-duplicate)
- Missing and empty questions
- Question length and word count analysis
- Comparison of text characteristics across classes

### 📌 Key Insight
Duplicate question pairs tend to:
- Have similar lengths
- Share a higher number of common words

This insight motivated the use of **similarity-based and overlap-based features**.

---

## 🧹 Text Preprocessing

Implemented a **custom text preprocessing pipeline** including:

- Lowercasing
- HTML tag removal
- Punctuation and special character removal
- Contraction expansion
- Whitespace normalization

These steps ensure **clean, consistent, and model-ready text**.

---

## 🧠 Feature Engineering

### 🔹 Basic Features
- Character length of each question
- Word count per question

### 🔹 Advanced Linguistic Features
- Common word count
- Unique word count
- Word overlap ratio
- Absolute word count difference
- Mean word count difference
- Token-level similarity metrics

### 🔹 Bag of Words (BoW)
- Used `CountVectorizer` to convert text into numerical vectors
- Generated BoW representations for both questions
- Combined BoW vectors with handcrafted numerical features to form the final feature matrix

---

## 🛠️ Tools & Libraries

- **Python**
- **Pandas**, **NumPy**
- **Scikit-learn**
- **Regular Expressions (re)**
- **BeautifulSoup**
- **Matplotlib / Seaborn**

---

## 🔄 Project Workflow

1. Data loading and sampling  
2. Exploratory Data Analysis (EDA)  
3. Text preprocessing  
4. Feature engineering (basic + advanced)  
5. Bag of Words vectorization  
6. Final feature matrix preparation  

---

## 🎯 Skills Demonstrated

- Exploratory Data Analysis (EDA)
- NLP text preprocessing
- Feature engineering for text similarity
- Bag of Words modeling
- Data cleaning and transformation
- Python-based ML workflows

---

## 🚀 Future Enhancements

- Replace BoW with **TF-IDF**
- Use **word embeddings** (Word2Vec, GloVe)
- Train ML models (Logistic Regression, XGBoost)
- Handle class imbalance techniques
- Extend to **transformer-based models** (BERT, SBERT)

---

## 💡 Why This Project Matters

This project reflects **industry-relevant NLP practices**, focusing on:
- Clean data
- Meaningful, explainable features
- Strong ML foundations

These principles are critical before moving to complex deep learning or transformer-based models.

⭐ If you find this project useful, consider starring the repository!
