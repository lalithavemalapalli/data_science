# 💳 Credit Card Approval Prediction
### *A Data-Driven Story of Trust, Risk, and Financial Inclusion*

---

## 📖 The Story Behind This Project

Every day, thousands of people walk into a bank or open an app and ask a simple question:

- *"Can I get a credit card?"*

Behind the scenes, banks must answer a much harder question:

- *"Can we trust this person to pay us back?"*

For decades, this decision was made by loan officers relying on gut instinct, limited paperwork, and unconscious biases. Today, data science gives us a better way — one that is faster, fairer, and more consistent.

This project tells the story of how we use **real-world applicant data** to build a machine learning model that predicts whether a credit card application should be **approved or rejected** — based not on gut feeling, but on patterns learned from thousands of past customers.

---

##  The Dataset

We work with two datasets provided by a financial institution:

| File | Description | Rows |
|------|-------------|------|
| `application_record.csv` | Personal & financial details of applicants | 4,38,557 |
| `credit_record.csv` | Monthly credit behavior of existing customers | 10,48,575 |

These two datasets are the **raw ingredients** of our story. Together, they tell us not just who the applicants are — but how they *behave* with credit.

### Key Columns at a Glance

**Application Record:**
- `CODE_GENDER`, `FLAG_OWN_CAR`, `FLAG_OWN_REALTY` — Who are they?
- `AMT_INCOME_TOTAL`, `NAME_INCOME_TYPE` — How do they earn?
- `DAYS_BIRTH`, `DAYS_EMPLOYED` — How old and experienced are they?
- `NAME_EDUCATION_TYPE`, `NAME_FAMILY_STATUS` — What is their background?

**Credit Record:**
- `MONTHS_BALANCE` — Time window of observation
- `STATUS` — The heartbeat of our story:

| Status | Meaning | Label |
|--------|---------|-------|
| `C` | Credit paid off | ✅ Good |
| `0` | No overdue | ✅ Good |
| `X` | No loan that month | ✅ Good |
| `1` | 1–29 days overdue | ⚠️ Risky |
| `2` | 30–59 days overdue | 🔴 Bad |
| `3` | 60–89 days overdue | 🔴 Bad |
| `4` | 90–119 days overdue | 🔴 Bad |
| `5` | 120–149 days overdue | 🔴 Bad |

---

##  Project Roadmap — Chapters of Our Story

This project is structured as **5 chapters**, each in its own notebook:

```
📁 credit-card-approval/
│
├── 📄 README.md                          ← You are here — The Prologue
│
├── 📓 data_merge_preprocessing.ipynb     ← Chapter 1: Where Two Worlds Meet
│   Merging datasets, cleaning data, handling missing values
│
├── 📓 eda_analysis.ipynb                 ← Chapter 2: Reading Between the Lines
│   Exploratory analysis, distributions, correlations, class balance
│
├── 📓 feature_engineering.ipynb          ← Chapter 3: Crafting the Right Clues
│   Creating new features, encoding, scaling, selection
│
├── 📓 ml_analysis.ipynb                  ← Chapter 4: Teaching the Machine to Decide
│   Model training, evaluation, comparison, and final insights
│
└── 📁 data/
    ├── application_record.csv
    └── credit_record.csv
```

---

##  How to Follow Along

Each notebook is designed to be **read like a story** — every code cell is preceded by a markdown cell explaining *why* we are doing what we are doing, not just *what* the code does.

You don't need to be a data scientist to follow along. If you've ever wondered how banks make decisions — this project shows you, step by step.

---

##  Tech Stack

| Tool | Purpose |
|------|---------|
| `Python 3.x` | Core language |
| `Pandas` | Data manipulation |
| `NumPy` | Numerical operations |
| `Matplotlib & Seaborn` | Visualizations |
| `Scikit-learn` | Machine learning models |
| `Jupyter Notebook` | Interactive storytelling environment |

---

##  What We're Trying to Predict

- **Binary Classification:**
- Given an applicant's personal, financial, and behavioral data —
- will they be a **Good** (repays on time) or **Bad** (defaults) credit card holder?

- `1` → Good Customer (Approve ✅)
- `0` → Bad Customer (Reject ❌)

---

##  Key Results (Spoiler — filled after ml_analysis.ipynb)

| Model | Accuracy | ROC-AUC |
|-------|----------|---------|
| Logistic Regression | — | — |
| Random Forest | — | — |
| Decision Tree | — | — |

*Results to be updated after completing ml_analysis.ipynb*

---

## Conclusion

- *This project was built not just to build a model, but to understand a process — the process of turning raw human data into a fair, explainable, and useful decision system. Every step was taken deliberately, with curiosity and care.*

---

*"Data is not just numbers. It's people's lives, told in rows and columns."*