🎓 Student Academic Performance Insights (Machine Learning Project)
📘 Introduction

This project focuses on building an intelligent system that analyzes various academic, behavioral, and lifestyle factors to estimate a student’s overall academic performance.
By learning patterns from real data, the model helps identify students who may need additional support and highlights factors that influence learning outcomes.

🎯 Project Goals

The main objectives of this system are:

To analyze student-related attributes (study habits, attendance, scores, etc.)

To classify the academic performance of students into categories such as A, B, C, D, and E

To visualize important relationships between input variables

To assist educators, institutions, and learners by offering predictive insights

🛠️ Technologies & Libraries

This project is implemented using:

Python

Pandas – for dataset handling

NumPy – numerical operations

Matplotlib & Seaborn – data visualization

Scikit-Learn – preprocessing, model building, and evaluation

RandomForestClassifier – main prediction model

📂 Dataset & Feature Overview

The model uses a variety of attributes grouped into three categories:

📘 Academic Metrics

Mid-Term Marks

Final Exam Marks

Average Assignment Marks

Quizzes Performance

Class Participation

Project Evaluation

Total Score

📙 Behavioral Indicators

Attendance Percentage

Weekly Study Hours

Stress Level (scale 1–10)

Average Sleep Duration

📗 Social/Background Factors

Engagement in Extracurriculars

Internet Availability

Parent Educational Background

Unnecessary personal fields are removed during preprocessing to ensure clean and unbiased data.

⚙️ Workflow Summary
1️⃣ Cleaning & Preprocessing

Dropping irrelevant columns

Handling missing information

Converting categorical fields into numeric values

Standardizing numerical features

2️⃣ Model Training

Splitting dataset into 80% training and 20% test data

Training the model using Random Forest

3️⃣ Evaluation

The model’s performance is validated using:

Accuracy

Classification Report

Confusion Matrix

Visual plots for interpretation

4️⃣ Visual Analysis

Some of the analytics included:

Correlation heatmap

Scatter plots between total score and final score

Stress vs Grade patterns

Study time trends

🔮 Making Predictions

The system can intake new student data and predict a grade.
Example usage:

student_sample = {
    'Attendance (%)': 90,
    'Midterm_Score': 75,
    'Final_Score': 80,
    'Assignments_Avg': 70,
    'Quizzes_Avg': 65,
    'Participation_Score': 80,
    'Projects_Score': 85,
    'Total_Score': 75,
    'Study_Hours_per_Week': 15,
    'Extracurricular_Activities': 1,
    'Internet_Access_at_Home': 1,
    'Parent_Education_Level': 2,
    'Stress_Level (1-10)': 5,
    'Sleep_Hours_per_Night': 7
}

print("Predicted Grade:", predict_grade(student_sample))

📊 Expected Outcomes

Model: Random Forest Classifier

Accuracy Range: ~80–90% (depends on dataset quality)

Output Grades: A, B, C, D, E

This project provides insights into how different attributes contribute to academic performance and highlights the factors that impact grades the most.

🚀 Future Improvements

Deploy the model as a web app using Flask or Streamlit

Add neural networks for improved prediction accuracy

Track progress across semesters using time-based modeling

Integrate feedback loops for continuous model improvement
