
# 🎓 Student Placement Prediction using Logistic Regression

## 📌 Project Overview

This project uses **Machine Learning and Logistic Regression** to predict whether a student is likely to get placed based on their academic and personal information.

The project demonstrates a complete classification workflow, from data preprocessing and model training to evaluation, saving the trained model, and creating a Streamlit-based prediction interface.

## 🎯 Objective

To build a Binary Classification model that predicts student placement status:

- `1` → Placed
- `0` → Not Placed

## 📊 Dataset Description

The dataset contains student information, including the following features:

| Feature | Description |
|---|---|
| Age | Student's age |
| Gender | Student's gender |
| Stream | Academic branch |
| Internships | Number of internships completed |
| CGPA | Academic CGPA |
| Hostel | Hostel status |
| HistoryOfBacklogs | Whether the student has a history of backlogs |
| PlacedOrNot | Target variable: placement status |

**Target variable:** `PlacedOrNot`

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Logistic Regression
- Pickle
- Streamlit
- Google Colab

## ⚙️ Project Workflow

1. **Data Loading:** Load the student placement dataset using Pandas.
2. **Data Preprocessing:** Apply One-Hot Encoding to categorical variables using `pd.get_dummies()`.
3. **Feature Selection:** Separate independent variables (`X`) and the target variable (`y`).
4. **Train-Test Split:** Divide the dataset into training and testing sets.
5. **Model Building:** Create and train a Logistic Regression classifier.
6. **Prediction:** Predict placement outcomes for test data and individual student inputs.
7. **Evaluation:** Evaluate the model using accuracy, confusion matrix, precision, recall, and F1-score.
8. **Model Saving:** Save the trained model using Pickle.
9. **Deployment:** Build a Streamlit interface to accept student details and display predicted placement status.

## 🤖 Model Used

### Logistic Regression

Logistic Regression is a supervised machine learning algorithm used for classification.

In this project, the model estimates the probability that a student will be placed and classifies the student into one of two classes.

## 📈 Model Performance

The Logistic Regression model achieved the following test results in the notebook:

| Metric | Result |
|---|---:|
| Accuracy | 68.75% |
| Correct predictions | 11 out of 16 test samples |

### Confusion Matrix

```text
[[4 1]
 [4 7]]
```

The confusion matrix indicates:

- 4 students from class 0 were correctly predicted.
- 1 student from class 0 was incorrectly predicted as class 1.
- 4 students from class 1 were incorrectly predicted as class 0.
- 7 students from class 1 were correctly predicted.

**Note:** These results are from the notebook's particular train-test split. The dataset and test sample are small, so this score should not be interpreted as a reliable estimate of real-world placement prediction performance.

## 🚀 Streamlit Application

The project also includes a Streamlit-based Student Placement Predictor.

Users can enter student details such as age, internships, CGPA, hostel status, backlog history, gender, and academic stream.

The application uses the saved Logistic Regression model to display a predicted placement status.

### Run the application

Install the required libraries:

```bash
pip install pandas numpy matplotlib scikit-learn streamlit
```

Ensure that the trained model file `placement_selection_model.sav` and the Streamlit application file `app.py` are available in your project directory.

Run the application:

```bash
streamlit run app.py
```

*The notebook contains the model training, saving, and Streamlit application code. If `app.py` has not been saved as a separate file, extract the application code from the notebook before running this command.*

## 📚 Key Learnings

- Understanding supervised learning and binary classification.
- Applying One-Hot Encoding to categorical data.
- Training and evaluating a Logistic Regression classifier.
- Interpreting model coefficients and intercept.
- Using classification metrics to evaluate predictions.
- Saving and loading a trained model with Pickle.
- Building a simple interactive ML application using Streamlit.

## 🔮 Future Improvements

- Train and evaluate the model using a larger dataset.
- Apply cross-validation for more reliable evaluation.
- Compare Logistic Regression with other classification algorithms.
- Improve feature preprocessing and model performance.
- Add probability estimates and more detailed prediction explanations.

## 🔗 GitHub Repository

[View the Student Placement Classification Project](https://github.com/SowmiyaSSakthi/ML_Classification)

## 👩‍💻 Author

**Sowmiya S. Sakthi**

This project was developed as part of my Machine Learning learning journey.
