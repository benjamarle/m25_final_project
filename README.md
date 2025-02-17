
# Bayesian Optimization for Credit Card Fraud Detection

## Explanation
This project applies machine learning to detect fraudulent credit card transactions. Using a **Random Forest classifier**, we identify patterns in transaction data that indicate fraud. **Bayesian optimization** is used to fine-tune the model’s hyperparameters, improving accuracy while minimizing false positives. The goal is to enhance fraud detection performance and reduce financial losses due to fraudulent activities.

## Data
We use the **Credit Card Fraud Detection dataset** from Kaggle ([link](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)). The dataset contains anonymized transaction records collected over two days from European cardholders, with 284,807 transactions, of which 492 (~0.17%) are fraudulent. The features have been transformed using **Principal Component Analysis (PCA)** to protect user privacy.

The data is not provided within this repository. Please download it from Kaggle and put in the main project directory with the name "creditcard.csv".

## Model
We use a **Random Forest classifier**, a robust ensemble learning method that combines multiple decision trees to improve accuracy and reduce overfitting. Random Forest was chosen due to its **interpretability, efficiency, and strong performance on imbalanced datasets**. 

## Hyperparameter optimization
To improve model performance, we optimize the following hyperparameters using **Bayesian optimization**:
- **Number of trees**: Controls the number of estimators in the forest.
- **Maximum depth**: Limits the depth of each tree to prevent overfitting.
- **Minimum samples per split**: Determines how many samples are required to split an internal node.
- **Maximum features**: Specifies the number of features considered when looking for the best split.

Bayesian optimization is chosen because it efficiently finds optimal hyperparameters by balancing exploration and exploitation, reducing the number of evaluations needed compared to grid or random search.

## Results
The optimized **Random Forest model** achieved high **precision and recall**, effectively identifying fraudulent transactions while minimizing false positives. The use of **Bayesian optimization** improved detection accuracy compared to baseline models. 

Key insights:
- The model correctly identifies most fraud cases while keeping false alarms low.
- Hyperparameter tuning significantly improves model performance.
- Future improvements could explore **deep learning** techniques and additional feature engineering.