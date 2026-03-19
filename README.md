# 🎬 Movie Review Sentiment Analysis

## 📌 Project Overview
This project is an end-to-end Natural Language Processing (NLP) machine learning pipeline designed to classify movie reviews as either **Positive** or **Negative**. It includes comprehensive text preprocessing, the training and evaluation of multiple classification models, and a user-friendly Graphical User Interface (GUI) for real-time sentiment prediction.

## ⚙️ Features
* **Text Preprocessing Pipeline:** Implements tokenization, stop-word removal, and lemmatization to clean the raw text data.
* **Feature Extraction:** Transforms cleaned text into numerical format for machine learning (using TF-IDF/Bag of Words).
* **Extensive Model Comparison:** Evaluates 8 different machine learning architectures to find the optimal performer.
* **Interactive GUI:** A built-in web interface that allows users to type in a movie review and instantly see the predicted sentiment.

## 🧠 Model Comparison & Evaluation
To ensure the highest accuracy, multiple classification algorithms were trained and evaluated. The models tested include:
1. Naive Bayes (`MultinomialNB`)
2. Logistic Regression
3. Random Forest Classifier
4. Support Vector Machine (`SVC`)
5. K-Nearest Neighbors (`KNeighborsClassifier`)
6. Decision Tree Classifier
7. Ensemble Classifier (with Logistic Regression as the final estimator)
8. Neural Network (`MLPClassifier`)

### Evaluation Metrics
The models were strictly evaluated and compared based on four key metrics:
* **Accuracy:** Overall correctness of the model.
* **Precision:** Accuracy of the positive predictions.
* **Recall:** Ability of the model to find all positive instances.
* **F1-Score:** The harmonic mean of precision and recall.

*Visual comparisons of these metrics can be found in the repository, including a **Performance Heatmap** and **Metric Bar Charts** (`

<img width="523" height="292" alt="image" src="https://github.com/user-attachments/assets/cd4d11fd-b380-4b1b-b527-ee6f12231cad" />
<img width="1348" height="672" alt="image" src="https://github.com/user-attachments/assets/52c46859-078f-45ea-b3e7-1a7281384910" />
<img width="1041" height="598" alt="image" src="https://github.com/user-attachments/assets/afd96835-2886-4c3d-bd43-cc07289ef54d" />

`).*

## 🏆 Best Model: Support Vector Machine (SVM)
After evaluating all models, the **Support Vector Machine (SVC)** emerged as the most robust and accurate model for this specific text classification task. 

### SVM Confusion Matrix Results
The model demonstrated excellent performance with a well-balanced distribution of true positives and true negatives, effectively minimizing misclassifications.

| | Predicted Negative | Predicted Positive |
| :--- | :--- | :--- |
| **Actual Negative** | 4350 (True Negative) | 611 (False Positive) |
| **Actual Positive** | 473 (False Negative) | 4566 (True Positive) |

## 💻 Graphical User Interface (GUI)
The project features a clean, interactive GUI deployed using Gradio. Users can input custom reviews and test the SVM model's predictive capabilities in real-time.

### Screenshots
* **GUI Interface (Empty):** <img width="1202" height="420" alt="image" src="https://github.com/user-attachments/assets/22f0b377-50c0-485e-9f7a-87da36328517" />

* **GUI Prediction Result (Positive/Negative):**
<img width="1216" height="557" alt="image" src="https://github.com/user-attachments/assets/a8d80e6b-9c38-4ad0-81fb-cdd82646019b" />
<img width="1196" height="562" alt="image" src="https://github.com/user-attachments/assets/fda069b4-0c02-4ad6-9561-f9122c778ce3" />



## 🚀 How to Run the Project
1. Clone this repository to your local machine.
2. Open the provided Google Colab Notebook (`.ipynb` file).
3. Ensure the required dataset and the saved `.pkl` files (model and vectorizer) are loaded into your environment.
4. Run the cells sequentially to see the data processing, model training, and to launch the Gradio GUI directly within the notebook.

## 🛠️ Technologies Used
* Python
* Scikit-Learn (Machine Learning Models & Metrics)
* NLTK (Natural Language Toolkit for Preprocessing)
* Gradio (GUI Framework)
* Pandas, NumPy, Matplotlib, Seaborn (Data Manipulation & Visualization)
