# Predictive-Analysis-for-Customer-Churn
This project aims to predict customer churn using a dataset containing various features about customer accounts, subscription details, usage patterns, and more. By leveraging machine learning techniques, the goal is to identify customers who are likely to churn, allowing businesses to take proactive measures to retain them.

## Project Overview
Customer churn is a significant challenge for subscription-based businesses. By predicting which customers are at risk of churning, companies can implement targeted strategies to enhance customer satisfaction and retention. This project involves several steps including data preprocessing, feature engineering, model training, evaluation, and making predictions on unseen data.

## Key Features
- AccountAge: The age of the user's account in months.
- MonthlyCharges: The amount charged to the user on a monthly basis.
- TotalCharges: The total charges incurred by the user over the account's lifetime.
- SubscriptionType: The type of subscription chosen by the user (Basic, Standard, or Premium).
- PaymentMethod: The method of payment used by the user.
- PaperlessBilling: Indicates whether the user has opted for paperless billing (Yes or No).
- ContentType: The type of content preferred by the user (Movies, TV Shows, or Both).
- MultiDeviceAccess: Indicates whether the user has access to the service on multiple devices (Yes or No).
- DeviceRegistered: The type of device registered by the user (TV, Mobile, Tablet, or Computer).
- ViewingHoursPerWeek: The number of hours the user spends watching content per week.
- AverageViewingDuration: The average duration of each viewing session in minutes.
- ContentDownloadsPerMonth: The number of content downloads by the user per month.
- GenrePreference: The preferred genre of content chosen by the user.
- UserRating: The user's rating for the service on a scale of 1 to 5.
- SupportTicketsPerMonth: The number of support tickets raised by the user per month.
- Gender: The gender of the user (Male or Female).
- WatchlistSize: The number of items in the user's watchlist.
- ParentalControl: Indicates whether parental control is enabled for the user (Yes or No).
- SubtitlesEnabled: Indicates whether subtitles are enabled for the user (Yes or No).
- CustomerID: A unique identifier for each customer.
- Churn: The target variable indicating whether a user has churned or not (1 for churned, 0 for not churned).

## Workflow
### Data Preprocessing:
- Handled missing values and outliers.
- Applied one-hot encoding to categorical features.
- Dropped the CustomerID column to prevent it from affecting the model training.
### Feature Engineering:
- Created new features to improve the model's predictive power.
### Feature Selection:
- Selected the most relevant features using techniques like SelectKBest.
### Model Training:
- Experimented with multiple machine learning algorithms including Logistic Regression, Random Forest, and XGBoost.
- Performed hyperparameter tuning using Grid Search to optimize model performance.
### Model Evaluation:
- Evaluated models using metrics such as accuracy, precision, recall, F1 score, and ROC AUC score.
### Predictions:
- Made predictions on the test data.
- Created a prediction_df dataframe containing CustomerID and predicted_probability for customer churn.
## Results
The final model achieved a ROC AUC score of 0.7298. Further optimization and feature engineering can help improve the model's performance.

## Files Included
- train_data.csv: The training dataset with customer features and churn labels.
- test_data.csv: The test dataset with customer features.
- test_predictions.csv: The predicted probabilities of churn for the test dataset.
