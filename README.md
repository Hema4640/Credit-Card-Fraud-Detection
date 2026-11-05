# Credit Card Fraud Detection Using Machine Learning

A machine learning project that identifies potentially fraudulent credit card transactions using a Random Forest classifier. The project focuses on handling highly imbalanced transaction data and evaluating model performance using classification metrics beyond accuracy.

## Project Overview

Credit card fraud detection is a challenging classification problem because fraudulent transactions represent only a very small proportion of total transactions. This project uses exploratory data analysis and machine learning techniques to distinguish legitimate transactions from fraudulent ones.

A Random Forest classifier is trained and evaluated to assess its ability to detect fraudulent transactions while minimizing false positives.

## Dataset

- **Total transactions:** 284,807
- **Fraudulent transactions:** 492
- **Legitimate transactions:** 284,315
- **Fraud proportion:** Approximately 0.173%
- **Classification type:** Binary classification

The dataset is highly imbalanced, making precision, recall, F1-score, and Matthews Correlation Coefficient (MCC) important evaluation metrics.

## Technologies Used

- **Programming Language:** Python
- **Data Processing:** Pandas, NumPy
- **Machine Learning:** Scikit-learn
- **Data Visualization:** Matplotlib, Seaborn
- **Environment:** Jupyter Notebook

## Project Workflow

1. **Data Loading and Exploration:** Loaded the transaction dataset and examined its structure, statistical properties, and class distribution.
2. **Exploratory Data Analysis:** Analyzed transaction amounts, class imbalance, and feature correlations using visualizations.
3. **Data Preprocessing:** Separated input features and target labels and divided the dataset into 80% training and 20% testing subsets.
4. **Model Development:** Implemented and trained a Random Forest classifier to distinguish fraudulent transactions from legitimate ones.
5. **Model Evaluation:** Assessed predictions using precision, recall, F1-score, Matthews Correlation Coefficient, and a confusion matrix.

## Model Performance

The Random Forest classifier achieved the following results on the held-out test dataset:

| Evaluation Metric | Score |
|---|---:|
| Precision | 97.5% |
| Recall | 78.6% |
| F1-Score | 87.0% |
| Matthews Correlation Coefficient (MCC) | 0.875 |

### Performance Analysis

- **Precision (97.5%):** A high proportion of transactions predicted as fraudulent were actually fraudulent.
- **Recall (78.6%):** The model successfully identified approximately 78.6% of actual fraudulent transactions.
- **F1-Score (87.0%):** Demonstrates the balance between precision and recall.
- **MCC (0.875):** Indicates strong overall classification performance while accounting for both classes.

These results highlight the model's ability to identify fraudulent transactions despite the significant class imbalance.

## Repository Structure

```text
Credit-Card-Fraud-Detection/
│
├── ML___Credit_Card_Fraud_Detection-.ipynb
└── README.md
```

## How to Run the Project

1. Clone the repository:

```bash
git clone https://github.com/Hema4640/Credit-Card-Fraud-Detection.git
```

2. Navigate to the project directory:

```bash
cd Credit-Card-Fraud-Detection
```

3. Install the required libraries:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```

4. Open the Jupyter Notebook:

```bash
jupyter notebook
```

5. Open `ML___Credit_Card_Fraud_Detection-.ipynb` and execute the notebook cells.

**Note:** Download the dataset separately and update its file path in the notebook if necessary.

## Future Enhancements

- Explore class imbalance handling techniques such as SMOTE and undersampling.
- Compare Random Forest with advanced classifiers such as XGBoost and LightGBM.
- Perform hyperparameter tuning to investigate potential performance improvements.
- Develop a real-time fraud detection application using Flask or FastAPI.

## Author

**D. Hema Sree**

- GitHub: [Hema4640](https://github.com/Hema4640)
- Project Repository: [Credit Card Fraud Detection](https://github.com/Hema4640/Credit-Card-Fraud-Detection)
