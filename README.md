# Task 3 - Decision Tree Classifier

## What I did
- Built a Decision Tree Classifier to predict whether a customer subscribes to a term deposit
- Used the Bank Marketing dataset (UCI ML Repository)

## Steps
- Loaded the dataset and explored the target variable (`y` — yes/no subscription)
- Checked for missing values
- Encoded categorical columns (job, marital, education, etc.) using one-hot encoding (`pd.get_dummies`)
- Split data into 80% training / 20% testing sets
- Trained a Decision Tree Classifier (`max_depth=4` to keep it interpretable and avoid overfitting)
- Evaluated performance using accuracy score and classification report
- Visualized the trained decision tree

## Results
- Accuracy: 91.24%
- Precision: 0.90, Recall: 0.91, F1-score: 0.91 (weighted average)

## Tools used
- `pandas` – data loading, cleaning, encoding
- `scikit-learn` – train/test split, Decision Tree model, evaluation metrics
- `matplotlib` – decision tree visualization

## Key takeaway
Categorical data needs to be encoded into numbers before a model can use it. Limiting tree depth (`max_depth`) keeps the model interpretable and helps prevent overfitting to the training data.
