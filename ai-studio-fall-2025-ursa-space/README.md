# AI Studio (Fall 2025) — Ursa Space Systems

**Foundation Models for Satellite Image Intelligence · SAR Image Classification: Icebergs vs. Vessels**

> This folder showcases **my individual contributions** to a **team** AI Studio project.
> It is not the full project. The complete work — every team member's notebooks, the master
> comparison notebook, figures, and the project write-up — lives in the team repository:
>
> **🔗 [matheath9/Ursa-Space-Systems-1B](https://github.com/matheath9/Ursa-Space-Systems-1B)**

---

## The Project (team context)

For the Fall AI Studio in the Break Through Tech AI program, a team of seven fellows partnered
with **Ursa Space Systems** to solve a real maritime-intelligence problem: distinguishing
**icebergs from vessels** in **Synthetic Aperture Radar (SAR)** satellite imagery.

- **Dataset:** [Statoil/C-CORE Iceberg Classifier Challenge](https://www.kaggle.com/competitions/statoil-iceberg-classifier-challenge) (Kaggle) — ~1,604 labeled training samples, ~8,424 test samples.
- **Inputs:** 2-channel SAR images (`band_1`, `band_2`), 75×75 pixels, normalized to [-1, +1]. Label `0 = ship`, `1 = iceberg`.
- **Team approach:** benchmark classical/baseline models (MLP, Logistic Regression, Random Forest, CNN, Gradient Boosting) against **transfer-learning** approaches using pretrained **ViT** and **ConvNeXT** embeddings — quantifying the value of foundation-model features for this task.

## My Contribution

My assigned role on the team was **model development and embedding-visualization preparation**.
The two notebooks here are the work behind that:

| Notebook | What it is | Status |
|---|---|---|
| [`notebooks/iceberg_classifier_milestone1_2.ipynb`](./notebooks/iceberg_classifier_milestone1_2.ipynb) | My end-to-end Milestone 1 & 2 notebook: EDA on the SAR imagery, a baseline **MLP** classifier, then **ViT** embedding extraction with dimensionality reduction (PCA/t-SNE/UMAP) and statistical analysis of the embedding space. | ✅ Fully executed — all outputs and figures render on GitHub |
| [`notebooks/mlp_model_colin.ipynb`](./notebooks/mlp_model_colin.ipynb) | My polished, standalone **MLP baseline** — a clean, reusable implementation with training, evaluation, and diagnostic plots (loss curve, ROC, confusion matrix, precision-recall). | ⚠️ Code complete, but committed **without saved outputs** — see note below |

### The baseline MLP, in brief
- **Input:** 11,250 features (75×75×2 SAR bands, flattened)
- **Hidden layers:** [512, 256, 128] with ReLU activation
- **Output:** single sigmoid unit (binary classification)
- **Training:** Adam (lr = 0.001), L2 regularization (α = 1e-4), early stopping (patience = 10)
- **Reported validation ROC-AUC:** ~0.985

> This baseline was one input into the team's broader baseline-vs-pretrained comparison. Any
> aggregate/leaderboard results belong to the team and are reported in the team repository.

## Running these notebooks

The notebooks expect the Statoil dataset, which is **not** included here (it's gated behind the
Kaggle competition). To run locally:

1. Download the data from the [competition data page](https://www.kaggle.com/competitions/statoil-iceberg-classifier-challenge/data) (or via the Kaggle API: `kaggle competitions download -c statoil-iceberg-classifier-challenge`).
2. Update the file paths in the **Configuration** cell near the top of each notebook.
3. Install dependencies: `numpy pandas matplotlib seaborn scikit-learn tensorflow keras torch torchvision jupyter pillow`.

> **Note on `mlp_model_colin.ipynb`:** this notebook is committed without cell outputs, so on
> GitHub it currently shows code but no rendered charts. To make it a stronger portfolio piece,
> re-run it end-to-end with the Kaggle data and commit the executed version so the ROC curve,
> confusion matrix, and metrics display inline. The milestone notebook already renders fully.

## Credit

This was a collaborative project. Full team and individual contributions are listed in the
[team repository README](https://github.com/matheath9/Ursa-Space-Systems-1B#-team-members).
The notebooks in this folder are my own authored work; all other project components are the
work of the team.

---

[⬅ Back to portfolio home](../README.md)
