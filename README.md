
# IndiaAI Hackathon Project: Complaint Classification

This repository contains the code for the **IndiaAI Hackathon** project, focused on classifying complaints reported on the National Cyber Crime Reporting Portal. The dataset consisted of reports written in Hinglish (a mix of Hindi and English). This README provides detailed instructions on how to preprocess the dataset, run the code, and understand the models used.

## 🚀 Project Overview

The goal of this project was to classify complaints into specific categories and subcategories using various machine learning and deep learning models. We aimed to achieve high accuracy, precision, recall, and F1 scores.

### Key Features
- **Text Preprocessing**: Tokenization, stop-word removal, stemming, and text cleaning.
- **Model Evaluation**: Logistic Regression, Random Forest Classifier, XGBoost, LSTM, and DistilBERT were implemented and compared.
- **Optimized Results**: Models were fine-tuned to maximize performance metrics.

---

## 📂 Dataset Preprocessing

The provided dataset contained the following columns:
1. **Category**: Main category of the complaint.
2. **Subcategory**: Subcategory of the complaint.
3. **Additional Crime Info**: Detailed description of the complaint (Hinglish text).

### Steps for Preprocessing:
1. **Tokenization**: Breaking the text into individual words or tokens.
2. **Stop-Word Removal**: Removing common words (like "is", "the") that do not contribute to the meaning.
3. **Text Cleaning**: Removing special characters, numbers, and extra spaces.
4. **Stemming**: Reducing words to their root form using libraries like `NLTK`.
5. **Label Encoding**: Converting categorical labels (categories/subcategories) into numerical values.

---

## ⚙️ Models Used

### 1. **Logistic Regression**
- A simple and interpretable baseline model.
- Results: Achieved decent accuracy but struggled with complex Hinglish text.

### 2. **Random Forest Classifier**
- Ensemble-based model using multiple decision trees.
- Results: Improved accuracy compared to Logistic Regression but was slower for large datasets.

### 3. **XGBoost**
- Gradient Boosting model optimized for speed and performance.
- Results: Delivered robust results with better precision and recall for certain classes.

### 4. **LSTM (Long Short-Term Memory)**
- A deep learning model designed for sequential data.
- Results: Performed well on Hinglish text by capturing context and dependencies in long sentences.

### 5. **DistilBERT**
- A transformer-based model fine-tuned for text classification.
- Results: Outperformed all other models in accuracy and F1 score, making it the top choice for deployment.

---


## 💻 How to Run the Project

### Prerequisites
- Python 3.8+
- Required libraries: `pandas`, `numpy`, `scikit-learn`, `xgboost`, `tensorflow`, `transformers`, and `nltk`.


## 🛠️ Future Work
- Enhance the preprocessing pipeline for better Hinglish text handling.
- Explore newer transformer-based models like RoBERTa or GPT for improved results.
- Deploy the DistilBERT model using a user-friendly interface.

---

## 🙌 Contributing
Feel free to fork the repository, create a branch, and submit a pull request for any enhancements or bug fixes.

---

## 📜 License
This project is licensed under the [MIT License](LICENSE).

---

## 🤝 Acknowledgments
Special thanks to the **IndiaAI Hackathon** team for providing this challenging opportunity. Libraries like `transformers`, `NLTK`, and `TensorFlow` played a crucial role in building this project.

