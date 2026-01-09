💳 Credit Card Fraud Detection using PySpark & Machine Learning

## 📌 Project Overview
Credit card fraud detection is a critical real-world problem due to the highly imbalanced nature of transaction data and the significant financial losses caused by fraudulent activities.

This project presents a scalable fraud detection system built using PySpark and Machine Learning, capable of efficiently processing large datasets.
A Streamlit-based web application is also developed to provide real-time fraud probability prediction and risk assessment.


## 🎯 Objectives
* Detect fraudulent credit card transactions accurately
* Handle highly imbalanced datasets
* Use PySpark MLlib for scalable machine learning
* Deploy an interactive Streamlit web application


## 📂 Project Structure

```
├── credit card fraud detction using pyspark and machine learning.ipynb
├── credit card fraud detection using pyspark and machine learning (streamlit).ipynb
├── README.md
```


## 📊 Dataset
* **Source:** Kaggle – ULB Credit Card Fraud Dataset
* **Link:** [https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

### Dataset Details
* European cardholders’ transactions (September 2013)
* 284,807 total transactions
* 492 fraud cases (highly imbalanced)
* Features:

  * `V1` – `V28` (PCA-transformed)
  * `Time`, `Amount`
* Target variable:

  * `0` → Legitimate transaction
  * `1` → Fraudulent transaction


## 🛠️ Technologies Used
* Python
* PySpark
* Spark MLlib
* Machine Learning Algorithms
  * Logistic Regression
  * Decision Tree
  * Random Forest
* Streamlit (Model Deployment)


## ⚙️ Methodology
### 1️⃣ Data Loading

* Dataset loaded using PySpark DataFrames for scalable data processing.

### 2️⃣ Data Preprocessing

* Handled class imbalance inherent in fraud detection
* Selected relevant features (`V1`–`V28`, `Amount`, `Time`)
* Feature vectorization using VectorAssembler
* Split data into training and testing sets

### 3️⃣ Model Training

* Trained multiple ML models using Spark MLlib:
  * Logistic Regression
  * Decision Tree
  * Random Forest

### 4️⃣ Model Evaluation

Models evaluated using standard performance metrics:

* Accuracy
* Precision
* Recall
* F1-Score
* ROC–AUC

### 5️⃣ Deployment

* Best-performing model deployed using Streamlit
* Users input transaction details via sliders and numeric fields
* The app predicts:

  * Fraud Probability (%)
  * Risk Level (Low / Medium / High)


## 🚦 Risk Classification Logic
Based on predicted fraud probability:

* 🟢 **Low Risk** – Safe transaction
* 🟠 **Medium Risk** – Monitor closely
* 🔴 **High Risk** – Potential fraud detected

This risk-based output improves interpretability and real-world usability.


## 🖥️ Streamlit Application (UI / UX)


### Features

* Interactive and user-friendly interface
* Real-time fraud probability prediction
* Clear visual risk classification


## 📌 Key Learnings
* Handling imbalanced datasets
* Scalable ML using PySpark
* End-to-end ML pipeline development
* Deploying ML models with Streamlit


## 🔮 Future Enhancements
* Apply advanced imbalance techniques (SMOTE, ADASYN)
* Explore deep learning approaches
* Integrate real-time transaction streaming using Apache Kafka

