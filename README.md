ALGORITHM
 Step 1: Load Dataset
 ● Import the churn.csv dataset using pandas.
 Step 2: Handle Missing Data
 ● Fill missing numeric values with column means.
 Step 3: Encode Categorical Variables
 ● Applyone-hot encoding to convert categorical variables into numeric format.
 Step 4: Separate Features and Target Variable
 ● Split the dataset into features (X) and the target column (y).
 Step 5: Train-Test Split
 ● Divide the data into training (80%) and test (20%) sets using train_test_split.
 Step 6: Train Random Forest Model
 ● Initialize and fit a RandomForestClassifier on the training data.
 Step 7: Evaluate Model
 ● Predict on the test data.
 ● Calculate metrics:
 ○ Accuracy: Overall correct predictions.
 ○ Precision: Correct positive predictions out of all positive predictions.
 ○ Recall: Correct positive predictions out of all actual positives.
 ○ F1Score: Harmonic mean of precision and recall.
 ○ ROCAUC:Model'sability to separate classes.
 Step 8: Perform Hyperparameter Tuning
 ● UseGridSearchCV to find the best parameters (e.g., number of estimators,
 depth, and splits).
 Step 9: Train Best Model
 ● Fit the model using the best parameters identified in the tuning step.
Step 10: Save the Best Model
 ● Savethe trained model as best_rf_churn_model.pkl using joblib.
 Step 11: Analyze Feature Importance
 ● Extract and rank features by importance to understand the factors influencing
 churn.
 Step 12: Build a Tkinter GUI
 ● Create a user-friendly interface to:
 ○ Display model metrics.
 ○ Highlight top features influencing churn.
 ○ Provide actionable insights based on feature importance.
 Step 13: Load the Saved Model
 ● Reload the saved .pkl file to make predictions on new data.
 Step 14: Preprocess New Data
 ● Ensure new input data matches the format of the original dataset (e.g.,
 encoding categorical variables).
 Step 15: Predict Churn
 ● Usetheloaded model to predict if a customer will churn. Display results in the
 GUI.
 Step 16: Validate Results
 ● Comparepredictions with real outcomes (if available) for validation
