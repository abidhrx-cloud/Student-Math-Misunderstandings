Student Math Misunderstandings Detection

This project focuses on identifying the underlying misconception behind a student's incorrect answer in mathematics multiple-choice questions using machine learning techniques.

Problem Statement

Students often select incorrect answers due to specific conceptual misunderstandings rather than random guessing.

The objective of this project is to:

Identify the most probable misconception

Predict the top 3 possible misconceptions

Support automated and data-driven educational feedback systems

This task is formulated as a multi-class classification problem evaluated using Mean Average Precision at 3 (MAP@3).

Dataset Description

The dataset contains:

QuestionId

MC_Answer (selected option)

CorrectAnswer

Student Response

Misconception Label

The goal is to correctly predict the misconception label associated with each incorrect response.

Methodology
1. Exploratory Data Analysis

Analyzed distribution of misconception categories

Examined question-wise answer trends

Studied class imbalance across labels

2. Feature Engineering

Encoded categorical variables

Generated structured features from answer patterns

Designed ranking-based prediction outputs

3. Model Development

Trained a supervised multi-class classification system

Generated top-3 ranked predictions per instance

4. Evaluation Metric

Mean Average Precision at 3 (MAP@3)

Validation Performance:

Validation MAP@3: 0.83

Results

The system achieved a validation MAP@3 score of 0.83, demonstrating strong ranking performance in predicting the most relevant misconceptions.
