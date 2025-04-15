# 🗳️ Candidate Test 2022 - Political Data Analysis

This project explores data from the 2022 Danish parliamentary candidate tests, published by two major TV networks: **DR** and **TV2**. The aim is to analyze ideological positions, voting tendencies, party cohesion, and candidate classifications using machine learning.

## 📁 Contents

- `alldata.xlsx`: Combined responses from both DR and TV2.
- `drdata.xlsx`: Responses from DR candidates.
- `drq.xlsx`: DR questions.
- `tv2data.xlsx`: Responses from TV2 candidates.
- `tv2q.xlsx`: TV2 questions.
- `electeddata.xlsx`: Responses from elected candidates.

- `candidate_analysis.ipynb`: Jupyter Notebook with data preprocessing, exploration, and classification model development.
- `README.md`: Documentation of the project.

## 🎯 Objectives

This assignment involves a mix of exploratory data analysis (EDA), statistical interpretation, and supervised machine learning. The core tasks include:

- 🧓 **Age Distribution**: Analyze candidate age grouped by political party.
- 💬 **Confidence Score**: Identify the most “confident” candidates based on their use of extreme responses (±2).
- 🔍 **Response Variability**:
  - Intra-party differences: Identify which parties have the most internal disagreements.
  - Inter-party differences: Compare party stances on key issues.
- 🤖 **Party Classification Models**:
  Train and evaluate three models to predict party affiliation:
  - Decision Tree
  - Random Forest
  - Gradient Boosted Tree (e.g., using `xgboost` or `sklearn.ensemble.GradientBoostingClassifier`)
- 🧭 **Ideological Drift**: Identify candidates whose views deviate from their party's general position.

## 🗃️ Dataset Summary

All responses are on a **5-point Likert scale**: -2 (Strongly Disagree) to +2 (Strongly Agree). Some candidates participated in both tests, while others only took one.

Special considerations:
- **electeddata.xlsx** excludes 9 elected members (e.g., Mette Frederiksen, Lars Løkke), who did not participate.
- Each dataset requires standardization and alignment before comparative analysis.

## 🧪 Tools & Libraries

- Python 3.x
- Jupyter Notebook
- pandas, numpy
- seaborn, matplotlib
- scikit-learn
- xgboost (optional for gradient boosting)
- plotly (optional for interactive visuals)

## 🎨 Party Metadata

Each party is identified by a unique letter and associated with a political position and color for visualization:

| Party | Name (EN) | Political Position |
| :-: | ------------------------- | ---------------- |
| A | Social Democrats           | Centre-left      |
| V | Danish Liberal Party       | Centre-right     |
| M | Moderates                  | Centre-right     |
| F | Socialist People's Party   | Left-wing        |
| D | Denmark Democrats          | Right-wing       |
| I | Liberal Alliance           | Right-wing       |
| C | Conservative People's Party| Right-wing       |
| Æ | Red-Green Alliance         | Far-left         |
| B | Social Liberal Party       | Centre-left      |
| D | New Right                  | Far-right        |
| Z | The Alternative            | Centre-left      |
| O | Danish People's Party      | Far-right        |
| G | Free Greens                | Centre-left      |
| K | Christian Democrats        | Centre-right     |

*Note: Use the provided color palette (`image-1.png`) to maintain consistency in your visualizations.*

## 🧭 Analysis Inspiration

You can explore related work for inspiration and validation:

- [Kandidattest 2022 Overview](https://v2022.dumdata.dk/)
- [Candidate Test Deep Dive](https://kwedel.github.io/kandidattest2022/)
- [Political Landscape 2019](https://kwedel.github.io/kandidattest2019/)

## 🗂️ Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/nural7h/candidate-test-machine-leaning
