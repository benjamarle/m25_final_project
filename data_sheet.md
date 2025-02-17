# Data Sheet

## Motivation
- **Purpose**: The dataset was created to support research in fraud detection, specifically for training machine learning models to identify fraudulent credit card transactions.
- **Creators**: The dataset was collected and published by researchers from the Machine Learning Group at Université Libre de Bruxelles (ULB).
- **Funding**: The dataset was developed for academic research and was not funded by any specific company or commercial entity.

## Composition
- **Instances Representation**: The dataset contains records of credit card transactions, each represented by numerical features extracted using PCA to anonymize sensitive data.
- **Number of Instances**: The dataset consists of 284,807 transactions, with 492 labeled as fraudulent (~0.17% of the total).
- **Missing Data**: No missing values are reported, as the dataset was preprocessed before publication.
- **Confidentiality**: The dataset does not contain personally identifiable information, as all transaction details have been anonymized.

## Collection Process
- **Acquisition**: Transactions were collected from European credit cardholders over a two-day period in September 2013.
- **Sampling Strategy**: The dataset represents a highly imbalanced class distribution, with fraud cases being a very small percentage of total transactions.
- **Time Frame**: The data was collected over two consecutive days.

## Preprocessing/Cleaning/Labeling
- **Preprocessing**: The dataset was processed using PCA transformation to anonymize sensitive transaction details, and no raw unprocessed data is available.
- **Cleaning**: The dataset does not contain missing values, and all features have been standardized.
- **Labeling**: Fraudulent transactions were identified and labeled as '1', while legitimate transactions were labeled as '0'.
- **Raw Data Availability**: The original unprocessed transaction details are not available due to privacy concerns.

## Uses
- **Potential Uses**: The dataset can be used for various fraud detection techniques, anomaly detection, and imbalanced learning research.
- **Ethical Considerations**: Due to class imbalance, models trained on this dataset should be carefully evaluated to avoid bias and ensure fair treatment across transaction types.
- **Limitations**: The dataset reflects transactions from European cardholders only, and its generalizability to other regions or financial systems is uncertain.
- **Restricted Uses**: The dataset should not be used for identifying individuals or making financial decisions without proper evaluation and fairness assessments.

## Distribution
- **Availability**: The dataset is publicly available on Kaggle ([link](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)).
- **Licensing**: The dataset is open for research purposes but should be used in compliance with Kaggle's terms of use.

## Maintenance
- **Maintainers**: The dataset is maintained by the Machine Learning Group at Université Libre de Bruxelles, but no active updates or modifications are expected.