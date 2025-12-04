# CBS-AML-PROJECT

This is the repository for our Applied Machine Learning group project at CBS.

## ✅ Quick Start (after you’ve accepted the invite)

1. Open the repo: https://github.com/torbenbillow/CBS-AML-PROJECT
2. Open our starter notebook in Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](
https://colab.research.google.com/github/torbenbillow/CBS-AML-PROJECT/blob/main/notebooks/00_welcome.ipynb)

> [For your first time in Colab with our private repo] You must navigate to http://colab.research.google.com/github and allow access to **private repositories**.

3. Work in Colab. Run cells (Shift+Enter), make edits.
4. Save back to GitHub: **File → Save. 
   - **Repository:** `torbenbillow/CBS-AML-PROJECT`
   - **Branch:** create one, e.g. `feature/<your-name>-eda`
   - **Path:** keep notebooks under `notebooks/`
   - **Commit message:** short description of your changes
5. Open a Pull Request and request a review. We merge into `main` via PRs only.

---

## 🧭 Team Workflow (Colab + GitHub)

- **Open from badge** so you’re on the latest version.
- **One branch per task/person** (e.g., `feature/torben-cleaning`).
- **Small, frequent commits**; then open a **PR** for feedback/merge.
- Optional: before saving to GitHub, **Edit → Clear all outputs** in Colab to keep diffs small.


## 📂 Project Structure
- `notebooks/` — Jupyter notebooks for experiments and analysis.


QUESTIONS WE STILL HAVE: 
   1. Should we manually tune hyperparameters somehow? As in, we run through various combinations of hyperparameters for a given model, and then manually look at the evaluation results, and choose different parameter values? The whole elbow concept of minimizing the loss.
        - Should we do something other than GridSearchCV?
   2. How is preprocessing inside of each CV fold preventing data leakage?
   3. Should we use different evaluation metrics?
         - The evaluation metrics should be chosen based on the model or the dataset or both?
   4. When you're doing cross validation, is each fold's result somehow averaged or aggregated? For example, if we are doing linear regression, the data is split into 5 folds, each with 80/20 split. The model is trained 5 times, which produces (in this regression example) 5 regression equations with different coefficients. How do we then arrive at the "final" model?
   5. WE CANT FORGET TO INCLUDE THE OTHER DATASET.
   6. How is onehotencoder better than get_dummies?
   7. Do we need to consider dimension reduction (PCA, anything else?)
