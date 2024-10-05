# CompanyB_Case_Study
## Home-Credit Default Risk Competition by Kaggle
## Link: <https://www.kaggle.com/competitions/home-credit-default-risk/>
### This project is assigned for Data Scientist position by Company B and due date is 1 week. All works and project is prepared and submitted in 7 days.
### Assignment : Assignment_Home_Credit_Default_Risk.pdf
### Dataset is in the Kaggle Link. In order to use dataset, save it as "home-credit-default-risk" folder. Main dataset is called "application_train.csv". Useful features are aggregated from adjunctive datasets "bureau.csv", "bureau_balance.csv", "credit_card_balance.csv", "installments_payments.csv", "POS_CASH_balance.csv", "previous_application.csv"
### Main : Home_Credit_Default_Risk_main.ipynb
#### Due to time constraint, some of additional datasets are not used, skipped. 
#### Aggregated features are calculated using scripts "Preprocess_balance", "Preprocess_credit_card_balance", "Preprocess_pos_cash", "Preprocess_previous_application" and unique(SK_ID_CURR) aggregated features are saved as "balance_unique_preprocessed", "bureau_unique_preprocessed", "credit_card_unique_preprocessed", "previous_application_unique_preprocessed".
#### After aggregation, preprocessing is applied, ie handling NaN Values. Preprocessed data saved as "Xdata_preprocessed". Then Ridge Classifier and Cat Boost Classifier are trained. Imbalanced data is handled by adding class/sample weights. Feature Importances are calculated and saved. Hyperparameter Optimization including feature selection is applied using Optuna. Best models are saved. Shapley values are analyzed. 
#### Test predictions on test data "application_test.csv" are submitted as "kaggle_test_predictions". Best Cat Boost Classifier Model is used for the purpose. 
