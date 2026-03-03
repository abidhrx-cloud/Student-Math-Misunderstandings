# Student Math Misunderstandings Detection

An end-to-end machine learning project focused on identifying conceptual misconceptions behind incorrect student responses in mathematics multiple-choice assessments.

---

## Overview

Incorrect answers in mathematics often reflect specific misunderstandings rather than random mistakes.

Detecting these misconceptions enables targeted feedback and personalized learning interventions.

This project builds a predictive system that ranks the most likely misconceptions associated with each incorrect student response.

The system is evaluated using Mean Average Precision at 3 (MAP@3), a ranking-based metric suitable for top-k prediction tasks.

---

## Objective

- Predict the most relevant misconception for each incorrect answer
- Generate top-3 ranked predictions per student response
- Optimize performance using a ranking-based evaluation framework

---

## Dataset

The dataset consists of structured student response records including:

- QuestionId
- MC_Answer
- CorrectAnswer
- Student Response
- Misconception Label

The task is formulated as a multi-class classification problem with ranking-based output evaluation.

---

## Methodology

### Data Analysis

- Examined distribution of misconception labels
- Identified imbalance across categories
- Analyzed response patterns at question level

### Feature Engineering

- Encoded categorical variables
- Created structured features from response patterns
- Designed top-k ranking outputs

### Evaluation

Mean Average Precision at 3 (MAP@3)

Validation MAP@3: 0.83

---

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

---

## Project Structure

student-math-misunderstandings/

├── notebooks/
│   ├── EDA.ipynb
│   ├── training.ipynb
│   └── inference.ipynb
│
├── data/
│   ├── train.csv
│   └── test.csv
│
├── requirements.txt
└── README.md

---

## How to Run

Install dependencies:

pip install -r requirements.txt

Run training:

python train.py

---

## Key Learnings

- Multi-class classification
- Implementation of MAP@K evaluation metrics
- Ranking-based prediction systems
- Handling imbalanced datasets
- End-to-end ML workflow development

---

## Future Improvements

- Improve ranking calibration
- Enhance feature representation
- Deploy as a web-based educational tool
- Integrate real-time prediction capabilities
