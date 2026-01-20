# Feature Encoding & Scaling

This project demonstrates feature encoding and scaling techniques applied to the Adult Income dataset to prepare data for machine learning models.
The focus of this work is on preprocessing steps such as handling missing values, encoding categorical features, and scaling numerical features to ensure model readiness.

## Dataset

- Adult Income Dataset
The dataset contains a mix of numerical and categorical features used to predict whether an individual's income exceeds $50K per year.

## Preprocessing Steps

- Identification of numerical and categorical features
- Handling missing values
- Label encoding for ordinal features
- One-hot encoding for nominal features
- Feature scaling using StandardScaler
- Comparison before and after scaling
- Export of preprocessed dataset

## Impact of Feature Scaling

- Feature scaling ensures that all numerical features contribute equally during model training.  
- It is especially important for distance-based and gradient-based algorithms such as KNN, SVM, and Logistic Regression.
- Tree-based algorithms are generally not affected by feature scaling.
- Negative values in the scaled dataset indicate values below the feature mean and are expected when using standardization.

## Note on Preprocessed Dataset

The complete preprocessed dataset is generated programmatically within the notebook.
Due to GitHub file size limitations, the full scaled CSV file is not included in this repository.  
Instead, a small sample file (`adult_income_preprocessed_sample.csv`) is provided for reference.

## How to Generate Full Dataset

To create the full preprocessed dataset (`adult_income_preprocessed.csv`):
1. Open `Adult_Income_Encoding_Scaling.ipynb` in Google Colab
2. Upload `adult_income.csv`
3. Run all cells
4. The processed CSV will be saved in the Colab file system

## Tools Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Google Colab
