# SDSC3006_Cityu

Coding assignments for **SDSC3006 Fundamentals of Machine Learning I** at City University of Hong Kong. The notebooks apply supervised learning methods from the [ISLP](https://islp.readthedocs.io/) stack (pandas, statsmodels, scikit-learn) to standard datasets.

This is my own coursework practice, shared for reference — please do not copy it for your assignments.

## Notebooks

| File | Topics |
| --- | --- |
| [`Assignment 1 coding.ipynb`](Assignment%201%20coding.ipynb) | Multiple linear regression on the **Carseats** data (`Sales` vs `Price`, `Urban`, `US`), plus a reduced model, 95% confidence intervals, and a residual-vs-fitted plot |
| [`Assignment 2 - Coding.ipynb`](Assignment%202%20-%20Coding.ipynb) | Classification on **Weekly** market direction: logistic regression, LDA, QDA, and KNN; leave-one-out CV for polynomial regression on simulated data |
| [`Assignment 3_coding.ipynb`](Assignment%203_coding.ipynb) | Regularization and dimension reduction on **College** (ridge, lasso, PCR); tree methods on **Carseats** (regression tree, pruning, bagging, random forest); further tree work on **OJ** |

Datasets are loaded with `ISLP.load_data` — nothing extra to download.

## Requirements

- Python 3 and [Jupyter](https://jupyter.org/)
- Packages used across the notebooks: `numpy`, `pandas`, `matplotlib`, `seaborn`, `statsmodels`, `scikit-learn`, `ISLP==0.3.19`
- Assignment 3 also installs `l0bnb` and pins `numpy==1.23.5` (see the first cell of that notebook)

Each notebook starts with a `pip install` cell. A clean virtual environment works too:

```bash
python3 -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install jupyter "ISLP==0.3.19" seaborn
jupyter notebook
```

Then open the assignment you want to run.

## Licence

MIT — see [LICENSE](LICENSE).
