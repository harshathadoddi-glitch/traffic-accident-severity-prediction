# Traffic Accident Severity Prediction

## 📌 Project Overview

Traffic accidents can result in different levels of injury, from slight injuries to serious or fatal injuries. Predicting accident severity using available accident-related information can help in understanding the factors associated with severe accidents.

This project uses **Machine Learning classification algorithms** to predict the severity of traffic accidents based on accident-related features.

The models are trained and evaluated using a traffic accident dataset, and their performance is compared using different classification metrics.

The **Weighted Random Forest** model was selected as the final model based on its performance.

---

## 🎯 Objectives

* Analyze traffic accident data.
* Perform data preprocessing and preparation.
* Identify useful features for accident severity prediction.
* Train multiple machine learning classification models.
* Compare the performance of the models.
* Select the best-performing model.
* Use the selected model to predict accident severity for new data.

---

## 📊 Dataset

The project uses a **Traffic Accident dataset** containing information related to road accidents.

The target variable represents the severity of the accident.

### Target Classes

* **Slight Injury**
* **Serious/Fatal**

The dataset was cleaned and prepared before applying machine learning algorithms.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook / Google Colab

---

## 🔄 Project Workflow

```text
Dataset
   ↓
Data Loading
   ↓
Data Cleaning
   ↓
Data Preprocessing
   ↓
Feature Selection
   ↓
Train-Test Split
   ↓
Model Training
   ↓
Model Evaluation
   ↓
Model Comparison
   ↓
Weighted Random Forest Selection
   ↓
Prediction on New Data
```

---

## 🤖 Machine Learning Models

Multiple classification models were trained and evaluated.

The models include:

1. Logistic Regression
2. Random Forest
3. Weighted Random Forest

The models were compared using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

---

## ⭐ Final Model: Weighted Random Forest

The **Weighted Random Forest** model was selected as the final model.

Class weighting was used to give more importance to the minority class. This is useful because the dataset contains an imbalance between the accident severity classes.

The final model was trained using the processed training data and evaluated on unseen test data.

---

## 📈 Model Evaluation

The performance of the models was evaluated using standard classification metrics.

### Evaluation Metrics

**Accuracy**

Measures the overall percentage of correctly classified observations.

**Precision**

Measures how many of the observations predicted as a particular class were actually members of that class.

**Recall**

Measures how many actual observations of a class were correctly identified.

**F1 Score**

Provides a balance between precision and recall.

**Confusion Matrix**

Shows the number of correct and incorrect predictions for each class.

---

## 📊 Results

The models were compared based on their evaluation metrics.

| Model                  |  Accuracy | Precision |    Recall |  F1 Score |
| ---------------------- | --------: | --------: | --------: | --------: |
| Logistic Regression    | 0.50      | 0.35      | 0.40      | 0.31      |
| Random Forest          | 0.85      | 0.62      | 0.33      | 0.31      |
| Weighted Random Forest | 0.85      | 0.62      | 0.34      | 0.31      |

> Replace the "Add value" entries with the actual values from your final model comparison results.

---

## 📉 Visualizations

The project includes visualizations such as:

* Model performance comparison
* Confusion matrix
* Feature importance
* Accident severity analysis

These visualizations help understand model performance and the factors contributing to accident severity prediction.

---

## 🔍 Feature Importance

Feature importance was analyzed using the Random Forest-based models to identify which input features contributed most to the predictions.

This helps provide a better understanding of the factors that are associated with accident severity.

---

## 🧪 Prediction on New Data

After training the final Weighted Random Forest model, it was tested on unseen test data.

Example:

```python
new_data = X_test.iloc[[0]]

new_prediction = rf_weighted.predict(new_data)

print(new_prediction)
```

The model returns the predicted accident severity class for the new observation.

---

## 📁 Project Structure

```text
traffic-accident-severity-prediction/
│
├── traffic_accident.ipynb
├── requirements.txt
├── README.md
└── images/
```

> The trained `.pkl` model file is not included in this repository because it exceeds GitHub's normal browser upload limit.

---

## ▶️ How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/harshathadoddi-glitch/traffic-accident-severity-prediction.git
```

### 2. Open the project

Open the project folder in Jupyter Notebook, JupyterLab, or Google Colab.

### 3. Install the required libraries

```bash
pip install -r requirements.txt
```

### 4. Open the notebook

Open:

```text
traffic_accident.ipynb
```

### 5. Run the notebook

Run the cells in order to:

* Load the dataset
* Preprocess the data
* Train the models
* Evaluate the models
* Compare their performance
* Generate visualizations
* Make predictions

---

## 💡 Key Findings

* Traffic accident severity can be modeled as a classification problem.
* Different machine learning models produce different levels of performance.
* Class imbalance can affect the prediction of minority accident-severity classes.
* A Weighted Random Forest can give greater importance to the minority class.
* Model evaluation should consider precision, recall, and F1 score rather than relying only on accuracy.

---

## 🚀 Future Improvements

Future versions of this project could include:

* Hyperparameter tuning using GridSearchCV or RandomizedSearchCV.
* Testing additional machine learning algorithms.
* Improving handling of class imbalance.
* Deploying the model as a web application.
* Adding real-time accident severity prediction.
* Using explainable AI techniques to better understand model predictions.

---

## 👩‍💻 Author

**Harshatha Doddi**

B.Tech – Computer Science and Data Science

---

## 📜 License

This project is created for educational and academic purposes.
