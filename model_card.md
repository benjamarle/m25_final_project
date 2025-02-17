# Model Card

## Model Description
- **Model Type**: Random Forest with Bayesian optimization for hyperparameter tuning.
- **Input Features**: Anonymized transaction features, amount, and time.
- **Optimization Goal**: Maximize fraud detection accuracy while minimizing false positives.

### **Model Architecture**
- **Feature Engineering**: Scaling and transformation of anonymized transaction features.
- **Classifier**: Random Forest consisting of multiple decision trees.
- **Hyperparameter Tuning**: Bayesian optimization to select the best combination of parameters such as the number of trees, maximum depth, and split criteria.
- **Prediction Output**: Binary classification (0: Legitimate, 1: Fraudulent).


### **Performance **
- **Precision**: High precision ensures fewer false positives.
- **Recall**: High recall ensures fraudulent transactions are detected.
- **F1-Score**: Balanced performance measure.


### **Trade-offs**
- **False Positives vs. False Negatives**: A model with high recall may increase false positives, leading to unnecessary investigations. Conversely, optimizing for precision might allow fraudulent transactions to go undetected.
- **Model Complexity vs. Interpretability**: More complex models may achieve higher accuracy but could be harder to interpret for decision-making.
- **Computation Time vs. Optimization**: Bayesian optimization improves model performance but increases computational cost.

### **Limitations**
- Highly imbalanced dataset; requires resampling techniques.
- Dependent on feature engineering due to anonymized variables.


### **Ethical Considerations**
- Preventing biased fraud classification.
- Transparent decision-making for flagged transactions.
