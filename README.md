# Optimized SVM Performance Evaluation Assignment

## 📌 Objective

This project aims to evaluate the performance of **Optimized Support Vector Machines (SVMs)** across multiple datasets using hyperparameter tuning. The goal is to determine the best SVM configuration for each sample and analyze the convergence behavior.

---

## 🧪 Methodology

### 1. **Data Preparation**
- Multiple data samples (S1 to S10) were used for experimentation.
- Each sample contains input features and labels suitable for binary or multi-class classification.

### 2. **Model Selection**
- **Support Vector Machine (SVM)** was selected due to its robustness and effectiveness in classification tasks.
- Kernels used: `linear`, `poly`, `rbf`, `sigmoid`.

### 3. **Hyperparameter Optimization**
- A randomized search strategy was used to explore combinations of:
  - **Kernel type**
  - **Regularization parameter (C)**: controls margin hardness.
  - **Epsilon (ε)**: used for epsilon-insensitive loss in regression or for controlling margins in classification.

### 4. **Evaluation Criteria**
- **Accuracy** was chosen as the primary performance metric.
- The best hyperparameter combination for each sample was selected based on the highest accuracy score over 100 iterations.

---

## 📊 Results

### 📌 Table 1: Comparative performance of Optimized-SVM with different samples

| Sample # | Best Accuracy (%) | Best SVM Parameters                         |
|----------|-------------------|---------------------------------------------|
| S1       | 100.00            | Kernel=poly, C=1.67, Epsilon=0.56           |
| S2       | 100.00            | Kernel=rbf, C=0.60, Epsilon=0.45            |
| S3       | 98.15             | Kernel=rbf, C=100.00, Epsilon=1.00          |
| S4       | 100.00            | Kernel=sigmoid, C=0.60, Epsilon=1.00        |
| S5       | 98.15             | Kernel=rbf, C=35.94, Epsilon=1.00           |
| S6       | 100.00            | Kernel=rbf, C=100.00, Epsilon=0.45          |
| S7       | 100.00            | Kernel=linear, C=0.01, Epsilon=0.34         |
| S8       | 100.00            | Kernel=linear, C=0.01, Epsilon=0.01         |
| S9       | 100.00            | Kernel=rbf, C=0.08, Epsilon=0.89            |
| S10      | 100.00            | Kernel=rbf, C=4.64, Epsilon=0.45            |

✅ **Observation**:
- The `rbf` kernel appears most frequently among the best-performing configurations.
- Models achieve excellent accuracy (98.15%–100%), demonstrating effective optimization.

---

## 📈 Result Graph

### Figure 1: Convergence graph of best SVM (S1)

![image](https://github.com/user-attachments/assets/742a44e0-deec-4ce6-ba9c-af0661f8c534)


- **X-axis**: Iteration number (1 to 100)
- **Y-axis**: Accuracy score
- The graph demonstrates how the optimization process converges, with most iterations yielding high accuracy.
- A few outlier configurations with low accuracy show the importance of proper hyperparameter selection.

---


## 📬 Contact

For queries or collaborations, feel free to connect!

---

