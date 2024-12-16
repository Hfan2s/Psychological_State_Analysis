# Psychological_State_Analysis

## Project Overview
This project analyzes and predicts the psychological states of individuals based on physiological, contextual, and demographic data. The dataset includes various attributes such as heart rate variability (HRV), EEG power bands, blood pressure, cognitive load, and more, which are used to train machine learning models for classification tasks.

## Purpose
The purpose of this project is to:
- Explore correlations between physiological metrics and psychological states.
- Build a predictive model to classify psychological states (e.g., Relaxed, Stressed, Anxious).
- Visualize feature importance and other key insights using interactive visualizations.

## Dataset
The dataset, `psychological_state_dataset.csv`, contains the following features:
- **Physiological Data**: HRV, GSR, EEG power bands, blood pressure, heart rate, skin temperature, and more.
- **Contextual Data**: Cognitive load, mood state, respiration rate, focus duration, and ambient noise levels.
- **Demographic Data**: Age, gender, educational level, and study major.

## Technologies Used
The project leverages the following technologies and libraries:
- **Python**: Programming language used for analysis and modeling.
- **Pandas**: For data manipulation and cleaning.
- **NumPy**: For numerical computations.
- **scikit-learn**: For preprocessing, model training, and evaluation.
- **Plotly**: For interactive visualizations of data and model results.
- **Jupyter Notebook**: For organizing and executing the code in a step-by-step manner.

## Steps in the Project
### 1. Data Loading
   - Load the dataset from the specified path.
   - Inspect the data structure using `.info()` and `.describe()`.

### 2. Data Cleaning
   - Handle missing values for both numerical and categorical columns.
   - Drop unnecessary features such as `ID` and `Time`.

### 3. Feature Engineering
   - Extract meaningful insights from complex columns like `EEG Power Bands`.
   - Encode categorical variables using `LabelEncoder`.

### 4. Feature Scaling
   - Normalize numerical features using `StandardScaler` to standardize the input data.

### 5. Model Training
   - Use a **Random Forest Classifier** to predict psychological states based on physiological and contextual data.
   - Split the data into training and testing sets for validation.

### 6. Model Evaluation
   - Evaluate the model using accuracy, precision, recall, and F1-score.
   - Generate a detailed classification report.

### 7. Visualization
   - Use Plotly to visualize:
     - Feature importance in predicting psychological states.
     - Distributions of mood and psychological states.

## How to Run the Project
### Prerequisites
1. Python (>= 3.8)
2. Required Python libraries:
   ```bash
   pip install pandas numpy scikit-learn plotly
