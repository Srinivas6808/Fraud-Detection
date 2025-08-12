# Fraud-Detection

## 📌 Overview
This project implements a **Fraud Detection Model** using **Machine Learning** to identify fraudulent transactions.  
The model uses a **Random Forest Classifier** trained on a dataset containing transaction details and is evaluated using standard classification metrics.

## 📂 Dataset
- The dataset used is `Fraud.csv` (replace with your actual dataset path).
- Contains transaction details such as:
  - `step` – Time step of the transaction
  - `type` – Type of transaction (encoded numerically)
  - `amount` – Transaction amount
  - `oldbalanceOrg` / `newbalanceOrig` – Balance before and after the transaction for the origin account
  - `oldbalanceDest` / `newbalanceDest` – Balance before and after the transaction for the destination account
  - `isFraud` – Target variable (1 = Fraudulent, 0 = Genuine)

## 🛠 Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/fraud-detection-model.git
   cd fraud-detection-model
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## 📜 Requirements
The main libraries used are:
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

You can install them using:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## 🚀 How to Run
1. Place the `Fraud.csv` file in the project directory.
2. Run the script:
   ```bash
   python fraud_detection.py
   ```
3. The script will:
   - Load and preprocess the data
   - Train a Random Forest model
   - Evaluate the model (confusion matrix, classification report, ROC curve)
   - Display feature importance

## 📊 Model Evaluation
The model evaluation includes:
- **Confusion Matrix**
- **Classification Report** (Precision, Recall, F1-Score)
- **ROC AUC Score**
- **ROC Curve**
- **Feature Importance Plot**

## 📈 Sample Outputs
- **ROC Curve**
  ![ROC Curve](roc_curve.png)
- **Top Feature Importances**
  ![Feature Importance](feature_importance.png)

## 🔮 Future Improvements
- Try other algorithms like **XGBoost** or **LightGBM**
- Perform **hyperparameter tuning** for better performance
- Handle **class imbalance** using SMOTE or other techniques
- Deploy the model as an **API** or integrate into a web dashboard

**Author:** Rasala Srinivas
