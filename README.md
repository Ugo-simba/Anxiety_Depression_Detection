# Anxiety_Depression_Detection
# README: Anxiety and Depression Detection Project

## *Project Overview*
This project focuses on detecting anxiety and depression in textual data using machine learning models, combining baseline and advanced approaches. The goal is to classify text into two categories: anxiety/depression or no anxiety/depression, with an emphasis on model explainability through tools like LIME.

## *Motivation*
Mental health issues, especially anxiety and depression, are on the rise, particularly among students. Identifying signs of these conditions in written text (e.g., social media posts) can enable early intervention. This project bridges the gap between advanced classification models and their interpretability, ensuring trust in their predictions for sensitive applications.

---

## *Key Objectives*
1. *Model Development:* Create robust models to classify anxiety and depression in text.
2. *Explainability:* Use LIME to interpret predictions at both global and local levels.
3. *Feature Analysis:* Identify key words or phrases that drive the model's decisions.
4. *Performance Comparison:* Compare baseline models like Logistic Regression with advanced models such as DistilBERT.

---

## *Dataset*
- *Source:* [Kaggle Dataset](https://www.kaggle.com/datasets/sahasourav17/students-anxiety-and-depression-dataset)
- *Details:* Contains 6,982 text samples labeled as:
  - 1 for anxiety/depression
  - 0 for no anxiety/depression

---

## *Project Workflow*
### 1. *Preprocessing*
- Handle missing values.
- Clean text (lowercase, remove links, punctuations, and emojis).
- Lemmatize text for better semantic accuracy.
- Address class imbalance using *SMOTE*.

### 2. *Feature Engineering*
- Compute sentiment scores.
- Extract word counts.
- Vectorize text using *TF-IDF* (unigrams and bigrams).

### 3. *Model Training*
- *Baseline Model:* Logistic Regression.
- *Advanced Models:* Random Forest, XGBoost, and DistilBERT (Transformer).
- Train-test split: 80%-20%.

### 4. *Evaluation Metrics*
- *Accuracy, Precision, Recall, F1-Score*
- *AUC-ROC Curve*
- Cross-validation to ensure generalizability.

### 5. *Explainability*
- Utilize *LIME* to highlight influential features in predictions for Logistic Regression and DistilBERT.

---

## *Results*
### Logistic Regression
- *Accuracy:* 98.4%
- *AUC:* 0.9968
- Suitable for interpretability but limited in handling complex patterns.

### Random Forest
- *Accuracy:* 99.28%
- *AUC:* 0.9988
- Strong performance with robust handling of data complexity.

### XGBoost
- *Accuracy:* 99.16%
- *AUC:* 0.9975
- Excellent generalization with minimal overfitting.

### DistilBERT
- To be completed as part of advanced model exploration.

---

## *Technologies Used*
- *Programming Language:* Python
- *Libraries:*
  - pandas, numpy, matplotlib, seaborn (Data processing and visualization)
  - nltk, spacy, TextBlob (Text preprocessing)
  - scikit-learn, imblearn (Modeling and evaluation)
  - lime, transformers (Explainability and Transformer models)

---

## *How to Use*
1. Clone the repository:  
   bash
   git clone <repository-link>
   
2. Install dependencies:
   bash
   pip install -r requirements.txt
   
3. Run the preprocessing and modeling scripts step-by-step as outlined in the notebook.

---

## *Future Work*
- Integrate more advanced models (e.g., BERT variations).
- Deploy the best-performing model as a web-based mental health tool.
- Expand to multilingual datasets for broader applications.

---

## *Authors*
- *Joanne Osuchukwu:* Preprocessing, advanced models, explainability.
- *Ugochukwu Ekwosimba:* Data cleaning, baseline models.

---


## *Acknowledgments*
Special thanks to Kaggle and contributors for providing the dataset.
