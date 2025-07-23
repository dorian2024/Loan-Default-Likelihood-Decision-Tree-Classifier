# Loan Default Prediction using Decision Tree Classifier

This project aims to predict the likelihood of a loan applicant defaulting using a **Decision Tree Classifier**. Built collaboratively by a team of three, the project walks through a complete machine learning pipeline—from data preprocessing to model evaluation and interpretation.

> ⚠️ Note: While the model demonstrates the process, its performance is not suitable for real-world deployment.

---

## Dataset

We used the [`application_train.csv`](https://www.kaggle.com/competitions/home-credit-default-risk/data) file from the **Home Credit Default Risk** dataset available on Kaggle.

---

## Project Workflow

### Data Understanding & Preprocessing
- Load and explore `application_train.csv`
- Handle missing values
- Encode categorical variables (Label Encoding & One-Hot Encoding)
- Perform data cleaning and type conversions

### Feature Engineering
- Removed unnecessary features
- Handled outliers and skewed distributions
- Scaled/normalized numeric features (where necessary)

### Model Training
- Split the data into **train / validation / test** sets
- Trained a **Decision Tree Classifier** using scikit-learn
- Tuned hyperparameters using **GridSearchCV**

### Model Evaluation
- Evaluated using:
  - Accuracy
  - Precision
  - Recall
  - F1 Score
  - ROC-AUC
- Plotted:
  - Confusion Matrix
  - ROC Curve (AUC = 0.71)
- Visualized tree using `plot_tree()`

### Optimization & Interpretation
- Applied pruning (depth limitation) to reduce overfitting
- Visualized **feature importance**
- Compared performance with **Random Forest Classifier**

### Finalization
- Saved the final model using `pickle`

---


## Limitations

- **Overfitting**: The decision tree memorized patterns from training data but struggled on data for class 1.

---

## Team Members

- Umaima Zeeshan
- Mehral Arif
- Taiba Tariq


---

## How to Run

1. Clone the repo:
    ```bash
    git clone https://github.com/dorian2024/Loan-Default-Likelihood-Decision-Tree-Classifier.git
    cd Loan-Default-Likelihood-Decision-Tree-Classifier
    ```

2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the notebook or Python script.

---



## License

This project is for academic purposes only.

