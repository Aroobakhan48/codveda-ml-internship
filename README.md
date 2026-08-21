# Codveda Technology — Machine Learning Internship
Six completed Machine Learning tasks for the Codveda Technology internship program (2 tasks per level, as required), covering the full pipeline from raw data to evaluated, interpretable models.

## Project Structure

| Level | Task | Folder | Dataset |
|---|---|---|---|
| 1 (Basic) | Data Preprocessing for ML | `Level1_Task1_Data_Preprocessing/` | Telecom Churn |
| 1 (Basic) | Simple Linear Regression | `Level1_Task2_Linear_Regression/` | Boston House Prices |
| 2 (Intermediate) | Logistic Regression | `Level2_Task1_Logistic_Regression/` | Telecom Churn |
| 2 (Intermediate) | Decision Tree Classifier | `Level2_Task2_Decision_Tree/` | Iris |
| 3 (Advanced) | Random Forest Classifier | `Level3_Task1_Random_Forest/` | Telecom Churn |
| 3 (Advanced) | Support Vector Machine (SVM) | `Level3_Task2_SVM/` | Telecom Churn |

Each folder is self-contained: its own `data/` subfolder with the required CSV(s), and a single Jupyter notebook with the complete workflow — load → preprocess → train → evaluate → visualize → summarize.

## Results Summary

- **Data Preprocessing:** Cleaned and encoded 3,333 customer records; produced a stratified 80/20 train/test split with all features scaled and ready for modeling.
- **Linear Regression (House Prices):** R² ≈ 0.67, RMSE ≈ 4.93 — `RM` (rooms) and `LSTAT` (% lower-status population) are the strongest predictors of price.
- **Logistic Regression (Churn):** Accuracy ≈ 0.78, AUC ≈ 0.83 — `Customer service calls` and `International plan` are the biggest churn drivers.
- **Decision Tree (Iris):** Accuracy ≈ 0.93 with a pruned tree (depth = 3) — `petal_length` and `petal_width` dominate the splits.
- **Random Forest (Churn):** Accuracy ≈ 0.96, F1 ≈ 0.86 — tuned via GridSearchCV with 5-fold cross-validation; confirms the same top churn drivers as logistic regression.
- **SVM (Churn):** RBF kernel achieves ≈ 0.90 accuracy and ≈ 0.93 AUC, clearly outperforming the linear kernel (≈ 0.77 accuracy) — indicating a non-linear decision boundary.

## Tools & Libraries

Python · pandas · NumPy · scikit-learn · matplotlib

## How to Run

```bash
pip install pandas numpy scikit-learn matplotlib
jupyter notebook
```

Open any task's `.ipynb` file and run all cells top to bottom. Each notebook reads its data via a relative `data/...` path, so keep the folder structure intact when running locally, or open each notebook individually in Google Colab and upload its matching `data/` files.

## Submission Checklist

- [x] All 6 tasks completed (2 per level)
- [x] Notebooks pushed to this repository
- [ ] Posted on LinkedIn per task, tagging **@Codveda** with `#CodvedaJourney #CodvedaExperience #FutureWithCodveda`
- [ ] Video explanation + this repo link included in each post
- [ ] Submitted via the official Codveda submission form
