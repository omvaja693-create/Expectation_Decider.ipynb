# 🎯 Expectation Decider

### A Beginner-Friendly Deep Dive into Probability, Random Variables & Bayes' Theorem — Powered by Real Student Data 📊

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-DataFrames-150458?logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557C?logo=plotly&logoColor=white)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)
![License](https://img.shields.io/badge/License-Educational-yellow)

---

## ✨ Overview

**Expectation Decider** is a hands-on probability and statistics project that answers a simple but powerful question:

> 🎓 *"Based on a student's study habits, attendance, and participation — what's the probability they'll pass their final exam?"*

Using a synthetic dataset of **200 students**, this project walks through core probability concepts step-by-step — from the absolute basics all the way to **Bayes' Theorem** — blending theory 📖 with practical Python implementation 🐍.

---

## 🗂️ Project Structure

| 📄 File | 📝 Description |
|---|---|
| `Expectation_Decider_Practical.ipynb` | The main Jupyter Notebook with all code, calculations & visualizations |
| `expectation_decider_dataset.csv` | Dataset of 200 students used throughout the analysis |
| `Theory.pdf` | Handwritten theory notes covering every probability concept used |
| `README.md` | You're reading it! 👋 |

---

## 📦 Dataset at a Glance

The dataset `expectation_decider_dataset.csv` contains **200 student records** with the following features:

| Column | Type | Description |
|---|---|---|
| `study_hours` | Numeric | Hours studied per week |
| `attendance` | Numeric (%) | Class attendance percentage |
| `group_discussion` | Categorical | Whether the student joined group discussions (`Yes` / `No`) |
| `previous_test_score` | Numeric | Score on a previous test |
| `final_exam_pass` | Categorical | Final result (`Pass` / `Fail`) 🎯 |

---

## 🧠 Concepts Covered

This project is structured as a progressive learning journey through probability 🚀:

### 1️⃣ Basics of Probability
- What is Probability? Formula: `P(A) = Favourable Outcomes / Total Outcomes`
- Key terminology: **Experiment**, **Sample Space**, **Event**, **Random Variable**, **Mutually Exclusive**, **Independent Events**, **Conditional Probability**

### 2️⃣ Empirical vs. Theoretical Probability
- **Empirical** 🔬 — calculated from real observed data (e.g. `P(Pass) = 45/100`)
- **Theoretical** 📐 — calculated from logical assumptions without needing experiments

### 3️⃣ Random Variables & Probability Distributions
- Built a discrete probability distribution for `X = 0, 1, 2, 3` passes
- Calculated:
  - **Expected Value** → `E[X] = Σ x·P(x) ≈ 2.14`
  - **Variance** → `Var(X) = Σ (x−μ)²·P(x) ≈ 0.631`

### 4️⃣ Venn Diagrams 🟢🔵
- **Set A** → Students studying more than 10 hrs/week
- **Set B** → Students attending more than 80% of classes
- Visualized overlaps using `matplotlib_venn` to find `P(A ∩ B)`, `P(A only)`, `P(B only)`, and `P(A ∪ B)`

### 5️⃣ Contingency Tables & Joint/Marginal/Conditional Probability 📋
Built a contingency table comparing `group_discussion` vs `final_exam_pass`:

|  | Pass | Fail | Total |
|---|---|---|---|
| **Group Discussion = Yes** | 90 | 30 | 120 |
| **Group Discussion = No** | 50 | 30 | 80 |
| **Total** | 140 | 60 | 200 |

- **Joint Probability** → `P(GD=Yes ∩ Pass) = 0.45`
- **Marginal Probability** → `P(Pass) = 0.70`
- **Conditional Probability** → `P(Pass | GD=Yes) = 0.75`

### 6️⃣ Understanding Relationships 🔗
Explored whether `group_discussion` and `final_exam_pass` are **independent**, **dependent**, or **mutually exclusive** — concluding they are **dependent**, since `P(Pass | Yes) ≠ P(Pass)`.

### 7️⃣ Bayes' Theorem Application 🧩
Given:
- `P(High Attendance | Pass) = 0.70`
- `P(High Attendance | Fail) = 0.40`
- `P(High Attendance) = 0.60`

Applied the **Law of Total Probability** to find `P(Pass) ≈ 0.667`, then applied **Bayes' Theorem** to compute:

> ### `P(Pass | High Attendance) ≈ 0.778` 🎉

**💡 Insight:** A student with high attendance (>80%) has roughly a **77.8% chance** of passing the exam!

---

## 🛠️ Tech Stack

- 🐍 **Python 3**
- 🐼 **Pandas** — data handling & contingency tables
- 🔢 **NumPy** — numerical computation
- 📊 **Matplotlib** & **matplotlib_venn** — visualizations & Venn diagrams
- 📓 **Jupyter Notebook** — interactive analysis

---

## ▶️ How to Run

1. Clone or download this repository 📥
2. Install the required libraries:
   ```bash
   pip install numpy pandas matplotlib matplotlib-venn
   ```
3. Make sure `expectation_decider_dataset.csv` is in the same folder as the notebook 📁
4. Launch Jupyter and run all cells:
   ```bash
   jupyter notebook Expectation_Decider_Practical.ipynb
   ```

---

## 🎥 Watch the Project Explainer Video

Want a full walkthrough of this project in action? Check out the explainer video below! 🍿

▶️ **[Watch on Google Drive](https://drive.google.com/file/d/1fcQQwSUjzYy1MMU64NerT1KZGuQWJ9_w/view?usp=sharing)**

---

## 📖 Theory Reference

All the underlying theory — probability definitions, formulas, worked examples, and step-by-step derivations — is documented in `Theory.pdf`, which pairs perfectly with the notebook's practical implementation. 📝

---

## 🌟 Key Takeaway

This project shows how **real, everyday questions** (like "will I pass my exam?") can be answered rigorously using probability theory — turning abstract formulas into meaningful, data-driven insights. 💡

---

<p align="center">Made with 💙, curiosity, and a lot of probability formulas</p>
