**Project: Diabetes Prediction using PySpark ML**

This project demonstrates how large-scale health data can be processed and analyzed using Apache Spark (PySpark) to predict diabetes outcomes. It was developed in Google Colab leveraging PySpark’s distributed data processing and machine learning libraries.

**Key Highlights**

**Data Ingestion & Exploration:**

Imported the Pima Indians Diabetes dataset from GitHub into a PySpark DataFrame.

Performed exploratory analysis including schema inspection, descriptive statistics, null/zero value detection, and class imbalance check (outcome distribution).

**Data Preprocessing:**

Handled missing and invalid data by replacing zero entries (in Glucose, Blood Pressure, Skin Thickness, Insulin, and BMI) with column mean values.

Computed feature correlations with the target variable to assess predictive significance.

Assembled multiple clinical attributes (e.g., Glucose, BMI, Insulin, Age) into a single feature vector using VectorAssembler.

**Model Development:**

Implemented Logistic Regression as a binary classifier to predict diabetes (Outcome = 1) or non-diabetes (Outcome = 0).

Split the dataset into 70% training and 30% testing for evaluation.

**Model Evaluation:**

Evaluated predictions using BinaryClassificationEvaluator.

Achieved ~82% accuracy, demonstrating the model’s effectiveness in medical outcome prediction.

**Model Persistence:**

Saved the trained logistic regression model using PySpark’s model.save().

Reloaded the model with LogisticRegressionModel.load() for future inference.

**Technologies & Tools**

**Google Colab** for development and execution.

**Apache Spark (PySpark)** for distributed data processing and ML.

**PySpark MLlib** for Logistic Regression and evaluation.

**GitHub dataset integration** for reproducible experimentation.

**Impact & Takeaway**

This project showcases how PySpark can handle large-scale healthcare datasets, perform efficient preprocessing, and build machine learning models for predictive analytics. It highlights practical skills in big data analytics, ML pipelines, and model lifecycle management.
