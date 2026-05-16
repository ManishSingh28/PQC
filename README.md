# Play-Quest-Conquer (PQC) — Game Success Prediction

A machine learning project built to help the **Play-Quest-Conquer** platform identify high-potential games before acquisition — using data to replace gut-feel in content procurement decisions.

---

## Problem

PQC needed a way to pre-screen games for their platform. Manually evaluating thousands of titles was slow, inconsistent, and expensive. The question: **can we predict whether a game will be well-received by users before committing to it?**

---

## Approach

Built an end-to-end ML pipeline on a dataset of 10,000+ board games, covering:

- Data cleaning and noise reduction (invalid years, missing player metrics)
- Exploratory data analysis across game types, age categories, complexity, and playtime
- Feature engineering and preprocessing (OneHot encoding for categorical variables)
- Model training and hyperparameter tuning using **Random Forest Regressor**
- Feature importance analysis to identify key drivers of user ratings
- Prediction pipeline applied to unseen competition data

---

## Results

| Metric | Value |
|---|---|
| Model | Random Forest Regressor |
| R² Score | 0.707 |
| Prediction Accuracy | 71% |
| Dataset Size | 10,000+ records |

**Top 2 drivers of user ratings: Complexity and Average Play Time**

These insights directly informed PQC's content procurement strategy — prioritising games with moderate-to-high complexity and longer engagement loops.

---

## Tech Stack

| Tool | Purpose |
|---|---|
| Python | Core language |
| Pandas | Data manipulation |
| Seaborn / Matplotlib | EDA and visualisation |
| Scikit-learn | Preprocessing, model training, evaluation |
| Google Colab | Development environment |
| Tableau | Dashboard export for business reporting |

---

## Dataset Features

| Feature | Description |
|---|---|
| `Released_Year` | Year the game was published |
| `Game_Type` | Base Game or Premium Game |
| `Age_Category` | Target age group |
| `Average_Complexity` | Community-rated complexity score (1–5) |
| `Average_Play_Time` | Expected session length in minutes |
| `Owner_Number` | Number of platform owners |
| `Rater_Number` | Number of users who rated the game |
| `Average_Rating` | Target variable — community average rating |

---


## Key Takeaways

- Complexity and Playtime are the strongest predictors of game ratings — not popularity or owner count
- Modular preprocessing pipelines handled noise at scale without manual intervention
- Model outputs were exported to Tableau for business-facing dashboards — bridging ML output with procurement decisions

---

## Author

**Manish Singh Chauhan**
IIT Patna | [LinkedIn](https://www.linkedin.com/in/manishchauhan28/)
