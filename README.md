# Matching-under-constraints

This repository contains the implementation of the project *"Matching under Constraints"* assigned in a course at École Polytechnique, under the supervision of Patrick Loiseau.

The project studies many-to-one matching problems (e.g. matching students to schools) under several types of constraints: **capacity constraints**, **group quotas**, **fairness rules (4/5-rule)**, and **budget limitations**. It also compares classical algorithms like Deferred Acceptance with more recent approaches such as the **Kamada-Kojima fixed-point algorithm**.

---

## 📘 Content

- `PI_Matching_GOMES_SELLES.ipynb`: Main notebook implementing and testing all algorithms for the various tasks in the project.
- `INF421-PI-MatchingConstraints-2024.pdf`: The original project specification.

---

## 📌 Objectives

The notebook is structured around the following major components of the project:

### ✅ Task 1–3: Deferred Acceptance Variants
- Implementation of the **Deferred Acceptance algorithm** with:
  - Capacity constraints
  - Group-based maximum quotas

### ✅ Task 4: Testing
- Testing the algorithms on:
  - Small fixed instance (Instance 1)
  - Randomized large instances (Instances 2 and 3) with student groups, costs, and noisy school preferences.

### ✅ Task 5–6: Fair Rankings (4/5-Rule)
- Preprocessing school preference lists to ensure that any prefix satisfies the 4/5-rule (up to 1 unit).
- Application of DA on modified rankings and verification of the fairness condition.

### ✅ Task 7–10: Kamada-Kojima Fixed-Point Algorithm
- Implementation of the fixed-point algorithm to find feasible, individually rational, and fair matchings under:
  - Capacity constraints
  - Group quotas
- Testing on all instances and discussion of failure under 4/5-rule.

### ✅ Task 11–14: Optimization under Budget Constraints
- Greedy or heuristic algorithms to:
  - Maximize the number of matched students (single school)
  - Minimize total student penalty (multiple schools)
- Respecting group fairness (4/5-rule) and cost budgets

---

## ⚙️ How to Run

This is a **Jupyter Notebook-based project**, written in Python.

### Dependencies

Install with:

```bash
pip install pandas numpy matplotlib tqdm

