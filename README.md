# Support Vector Regression (SVR) — Comparative Kernel Analysis

## 🎯 Problem Statement and Goal of Project

This project explores the application of **Support Vector Regression (SVR)** using different kernel functions (linear, polynomial, and RBF) on synthetic and real-world datasets. The main objective is to **understand how various SVR kernels perform** in modeling complex, non-linear data, rather than just optimizing accuracy.

---

## 🛠 Solution Approach

The notebook is structured in two parts:

### 1. **Synthetic Data Regression**

* **Dataset**: Random samples between 0 and 5.
* **Target**: Sine wave with added noise.
* **Goal**: Compare SVR kernels (`linear`, `poly`, `rbf`) in capturing underlying patterns.

### 2. **Real-World Dataset (Position Salaries)**

* **Source**: `Position_Salaries.csv`
* **Goal**: Predict salary based on job level using SVR with a Gaussian kernel.

### Steps Included:

* Data generation and noise injection.
* SVR model training with three different kernels.
* Visual comparison of predictions from each model.
* Second phase: Apply SVR on actual business data (position vs. salary).
* Basic data inspection using `pandas`.

---

## 🧰 Technologies & Libraries

* Python 3
* `numpy`, `pandas` — data manipulation
* `matplotlib`, `pylab`, `seaborn` — visualization
* `scikit-learn` — SVR models and utilities

---

## 📁 Dataset Description

* **Synthetic Dataset**:

  * `X`: Random numbers between 0 and 5
  * `y`: Sine values with added noise every 5th sample

* **Real Dataset**:

  * `Position_Salaries.csv`
  * Features: `Level` (numeric), `Salary`
  * Target: Salary prediction (continuous)

---

## ⚙️ Installation & Execution Guide

1. Ensure required files like `Position_Salaries.csv` are available.
2. Install necessary dependencies:

   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn
   ```
3. Run the notebook using:

   ```bash
   jupyter notebook SVR.ipynb
   ```

---

## 📊 Key Results / Performance

* The **RBF kernel** captured the **non-linear pattern** of the sine wave most effectively.
* **Linear kernel** underperformed on non-linear data (as expected).
* **Polynomial kernel** produced smoother curves but showed signs of overfitting in some regions.
* SVR on real data demonstrates its ability to generalize well with minimal tuning.

---

## 📸 Screenshots / Sample Outputs

* 🧪 Scatter plot of noisy sine data with all three regression curves.
* 📈 SVR performance visualization comparing kernel outputs.
* 📋 Sample extracted salary data from CSV file using `pandas`.

---

## 📚 Additional Learnings / Reflections

* This project focuses on **understanding kernel choice** and its effect on regression, **not maximizing metrics**.
* SVR provides robust control over **model complexity and margin violations** via the `epsilon` parameter.
* Combining **visual intuition** with **code-based experimentation** is key to mastering regression modeling.

---

## 👤 Author

## Mehran Asgari

**Email:** [imehranasgari@gmail.com](mailto:imehranasgari@gmail.com)
**GitHub:** [https://github.com/imehranasgari](https://github.com/imehranasgari)

---

## 📄 License

This project is licensed under the Apache 2.0 License – see the `LICENSE` file for details.

---

> 💡 *Some interactive outputs (e.g., plots, widgets) may not display correctly on GitHub. If so, please view this notebook via [nbviewer.org](https://nbviewer.org) for full rendering.*

---

