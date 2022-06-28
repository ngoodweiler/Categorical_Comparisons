# Categorical_Comparisons
Comparing different categorical modeling methods using real data from a processing facility

### Information about the dataset
- Data is collected from a real operating facility
- All labels have been modified to remove any sensitive information
- Dates from November 2020 through May 2022
- The first ~6 months of data was previously cleaned, however there are rows with missing or NaN values that must be addressed
- The process features and output are all *continuous* data, however the output will be set to 'Good', 'Warning', and 'Bad' categories (meaning a multiclass model is required)

### Methods to be compared
- Decision Tree
- Random Forest
- KNN
- Gaussian Naive Bayes
- Support Vector Machine
    - Linear
    - Poly
    - RBF

### Extra Notes
- Data will be standardized for KNN and SVM models using sklearn StandardScaler
- Feature selection will occur per model
- Initial cleaning will be performed and feature and outputs will be saved in separate CSV files to be utilized in separate notebooks for each model

## Final Results
- Out of 7 total models, Random Forest yielded the highest score of 0.742 and offered a medium level of interpretability
- The Radial Basis Function came in at a close second place with a score of 0.726, however it is more difficult to interpret how the model works
