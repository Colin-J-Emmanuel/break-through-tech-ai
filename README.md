# Break Through Tech AI — Portfolio

**Colin Emmanuel** · AI/ML Fellow, [Break Through Tech AI](https://www.breakthroughtech.org/) (hosted by **Cornell Tech**)

> A complete record of my work across the Break Through Tech AI program: the summer
> Machine Learning Foundations curriculum, the fall industry AI Studio with Ursa Space
> Systems, and a spring data-science competition. This repository is the home of my
> **individual Machine Learning Foundations coursework** (47 notebooks across 8 units)
> and the hub that links to my team AI Studio projects.

---

## Table of Contents

- [Program Overview](#program-overview)
- [The Three Phases at a Glance](#the-three-phases-at-a-glance)
- [Phase 1 — Machine Learning Foundations](#phase-1--machine-learning-foundations-summer-2025)
  - [What the Curriculum Covered](#what-the-curriculum-covered)
  - [Unit-by-Unit Breakdown](#unit-by-unit-breakdown)
  - [Highlighted Work](#highlighted-work)
- [Phase 2 — AI Studio with Ursa Space Systems](#phase-2--ai-studio-with-ursa-space-systems-fall-2025)
- [Phase 3 — WiDS Datathon: Wildfire Survival Forecasting](#phase-3--wids-datathon-wildfire-survival-forecasting-spring-2026)
- [Skills Demonstrated](#skills-demonstrated)
- [Repository Structure](#repository-structure)
- [Reproducing This Work](#reproducing-this-work)
- [A Note on Course Materials & Academic Integrity](#a-note-on-course-materials--academic-integrity)
- [About Me](#about-me)
- [Acknowledgements](#acknowledgements)
- [License](#license)

---

## Program Overview

[Break Through Tech AI](https://www.breakthroughtech.org/) is a national initiative that
prepares students for careers in artificial intelligence and machine learning through a
sequence of rigorous, hands-on experiences. As a Fellow in the program (hosted by Cornell
Tech), I moved through three connected phases:

1. **Machine Learning Foundations** — an intensive, project-based curriculum covering the
   full ML life cycle, from problem formulation to deep learning and NLP.
2. **AI Studio (Fall)** — a semester-long, team-based engagement solving a real problem for
   an industry partner, **Ursa Space Systems**.
3. **AI Studio (Spring)** — a second team engagement centered on a **Kaggle data-science
   competition**.

This repository documents all three, with the Foundations coursework hosted here in full and
the team projects linked to their respective repositories.

---

## The Three Phases at a Glance

| Phase | Term | Focus | Format | Where to find it |
|------|------|-------|--------|------------------|
| **1 · ML Foundations** | Summer 2025 | Full ML life cycle: data prep → classical models → deep learning → NLP | Individual coursework | **This repository** ⤵ |
| **2 · AI Studio — Ursa Space Systems** | Fall 2025 | SAR satellite-image classification (icebergs vs. vessels); transfer learning with ViT / ConvNeXT embeddings | Team (7 fellows) | [My notebooks ⤵](./ai-studio-fall-2025-ursa-space/) · [Team repo ↗](https://github.com/matheath9/Ursa-Space-Systems-1B) |
| **3 · WiDS Datathon — Wildfire Survival** | Spring 2026 | Survival analysis: forecasting wildfire threat to evacuation zones (12/24/48/72h); ensembling + calibration | Team (3) | [Project repo ↗](https://github.com/Colin-J-Emmanuel/wildfire-survival-forecasting) |

---

## Phase 1 — Machine Learning Foundations (Summer 2025)

The Foundations curriculum walks through the **complete machine learning life cycle** using
Python and the scientific-computing stack. Rather than isolated exercises, each unit builds
toward being able to take a raw dataset and a business question and deliver an evaluated,
deployable model — and to reason about its fairness and limitations.

This repository contains **47 of my completed notebooks**, organized into eight unit folders.
Within each unit, notebooks are grouped as:

- **`labs/`** — the graded, end-to-end lab for the unit (8 total, including the capstone)
- **`assignments/`** — the graded assignment for the unit (7 total)
- **`practice/`** — guided practice and demo notebooks that build individual skills (32 total)

### What the Curriculum Covered

| Stage of the ML Life Cycle | Where it lives |
|---|---|
| Business understanding & problem formulation | Unit 1 |
| Data understanding, cleaning, encoding, and feature preparation | Unit 2 |
| Classical supervised models (KNN, Decision Trees) | Unit 3 |
| Linear models (logistic & linear regression, gradient descent) | Unit 4 |
| Model evaluation, selection, cross-validation, and deployment | Unit 5 |
| Ensemble methods & unsupervised learning | Unit 6 |
| Deep learning & computer vision (neural nets, CNNs with Keras) | Unit 7 |
| Natural language processing & the capstone project | Unit 8 |
| Responsible ML: fairness, accountability, and readiness for production | Unit 9 *(theory)* |

### Unit-by-Unit Breakdown

Each unit links to its own README with a full notebook index and descriptions.

#### [Unit 1 — ML in a Nutshell](./unit-01-ml-in-a-nutshell/) · *5 notebooks*
The ML life cycle and the Python toolkit. Business understanding and problem formulation,
plus foundational practice with Jupyter, NumPy (vectorization & broadcasting), and pandas.
- **Lab:** ML Life Cycle — Business Understanding and Problem Formulation

#### [Unit 2 — Managing Data in ML](./unit-02-managing-data/) · *13 notebooks*
The largest hands-on unit. Data understanding and preparation end-to-end: filtering,
balancing classes, type handling, binary variables and one-hot encoding, exploratory
visualization with Seaborn/Matplotlib, summary statistics, and handling missing data and outliers.
- **Lab:** Data Understanding and Data Preparation
- **Assignment:** Preparing a Dataset for Modeling

#### [Unit 3 — Common Models: KNN & Decision Trees](./unit-03-common-models-knn-and-trees/) · *5 notebooks*
First supervised models. Implementing and optimizing k-Nearest Neighbors and Decision Trees,
then comparing them head-to-head.
- **Lab:** Modeling — Compare KNNs and Decision Trees
- **Assignment:** Train Decision Trees After Data Preparation

#### [Unit 4 — Linear Models](./unit-04-linear-models/) · *6 notebooks*
The mechanics beneath the models. Logistic regression built **from scratch**, the prediction
and evaluation loop, gradient descent, hyperparameter optimization, and linear regression on
the World Happiness Report.
- **Lab:** Logistic Regression From Scratch
- **Assignment:** Optimizing Logistic Regression

#### [Unit 5 — Evaluation & Deployment](./unit-05-evaluation-and-deployment/) · *7 notebooks*
Choosing and trusting a model. Cross-validation, model selection for both KNN and Decision
Trees, feature selection, the confusion matrix, and persisting a trained model for deployment.
- **Lab:** Model Selection for Logistic Regression
- **Assignment:** Model Selection for KNN

#### [Unit 6 — Ensembles & Unsupervised Learning](./unit-06-ensembles-and-unsupervised/) · *4 notebooks*
Beyond single models. Random Forests, Gradient Boosted Decision Trees, a comparison of
regression models, and an unsupervised clustering assignment.
- **Lab:** Compare Regression Models
- **Assignment:** Unsupervised Learning — Clustering

#### [Unit 7 — Deep Learning & Computer Vision](./unit-07-deep-learning-and-computer-vision/) · *3 notebooks*
Neural networks with Keras. Training a feed-forward network, implementing one from a
specification, and building a **Convolutional Neural Network** for image data.
- **Lab:** Implement a CNN with Keras
- **Assignment:** Implement a Neural Network with Keras

#### [Unit 8 — NLP & Capstone](./unit-08-nlp-and-capstone/) · *4 notebooks*
Text as data, and the capstone. Transforming text into features, word embeddings, a neural
sentiment classifier, and the **open-ended capstone** where I framed and solved an ML problem
of my own choosing.
- **Capstone (Lab 8a):** Define and Solve an ML Problem — *NLP sentiment analysis on book reviews*
- **Assignment:** Neural Network for Sentiment Analysis

#### [Unit 9 — Responsible ML](./unit-09-responsible-ml/) · *theory*
Preparing models for the real world: solution engineering, data sufficiency, feature issues,
and **fairness & accountability**. This unit is documented in a README summary (no notebooks).

### Highlighted Work

If you only look at a few notebooks, start here:

- **[Capstone — Define and Solve an ML Problem](./unit-08-nlp-and-capstone/labs/)** — the
  most self-directed piece: choosing a dataset, formulating the problem, and building an
  end-to-end sentiment-analysis solution on book-review text.
- **[Logistic Regression From Scratch](./unit-04-linear-models/labs/)** — implementing the
  model and its gradient-descent training loop without relying on a library's fit method,
  to show I understand what happens under the hood.
- **[Implement a CNN with Keras](./unit-07-deep-learning-and-computer-vision/labs/)** — a
  convolutional network for image classification, the deep-learning foundation that carried
  directly into the Ursa Space satellite-imagery project.

---

## Phase 2 — AI Studio with Ursa Space Systems (Fall 2025)

**📂 My notebooks in this repo: [`ai-studio-fall-2025-ursa-space/`](./ai-studio-fall-2025-ursa-space/)** · **🔗 Team repository: [matheath9/Ursa-Space-Systems-1B](https://github.com/matheath9/Ursa-Space-Systems-1B)**

**Foundation Models for Satellite Image Intelligence — SAR Image Classification: Icebergs vs. Vessels**

For the fall AI Studio, my team of seven fellows partnered with **Ursa Space Systems** to
tackle a real maritime-intelligence problem: distinguishing **icebergs from vessels** in
**Synthetic Aperture Radar (SAR)** satellite imagery, using the Statoil/C-CORE Iceberg
Classifier dataset from Kaggle.

**What the team built:**
- Baseline models (MLP, Logistic Regression, Random Forest, CNN, Gradient Boosting) benchmarked
  against **transfer-learning** approaches using pretrained **ViT** and **ConvNeXT** image embeddings.
- A baseline-vs-pretrained comparison methodology, with the baseline MLP reaching a **ROC-AUC of
  0.9855** on the held-out set.
- 3D PCA visualizations of the learned embedding spaces to analyze class separability.

**My contributions:** model development and **embedding-visualization preparation** — building a
baseline **MLP** classifier and turning high-dimensional pretrained (ViT) embeddings into
analyzable, comparable representations so the team could reason about how well each approach
separated the two classes. My authored notebooks (a fully-executed EDA + baseline + embeddings
notebook, and a standalone MLP baseline) are in
[`ai-studio-fall-2025-ursa-space/`](./ai-studio-fall-2025-ursa-space/), with details on what was
mine versus the team's.

*(The full write-up, aggregate results, figures, and every member's notebooks live in the team
repository linked above.)*

---

## Phase 3 — WiDS Datathon: Wildfire Survival Forecasting (Spring 2026)

**🔗 Project repository: [Colin-J-Emmanuel/wildfire-survival-forecasting](https://github.com/Colin-J-Emmanuel/wildfire-survival-forecasting)**

**Predicting Time-to-Threat for Wildfire Evacuation Zones — WiDS Global Datathon 2026, Survival Analysis Track**

For the Spring AI Studio, my three-person team entered the **Women in Data Science (WiDS) Global
Datathon 2026**, run on Kaggle in partnership with the wildfire-safety nonprofit
[Watch Duty](https://www.watchduty.org/). The task: given only the **first five hours** of a
wildfire's behavior, forecast the probability it threatens a nearby evacuation zone within **12, 24,
48, and 72 hours**. Because the outcomes are right-censored (many fires never reach a zone), it's a
**survival-analysis** problem rather than plain classification.

**Results:**
- Improved the provided XGBoost Cox baseline from **0.87397 → 0.96366** (**+0.09**), clearing the
  program's 0.90 target with margin.
- **Leaderboard: 477 / 1754 teams (top ~27%)** in a public, worldwide competition.

**What drove the gain:** early error analysis exposed that the baseline was **overconfident about
distant fires** — assigning real hit-probability to fires 7–545 km away, even though no training fire
ever reached a zone from beyond ~5 km. Correcting this was the biggest lever, through distance-aware
feature engineering and, above all, **per-horizon probability calibration** (isotonic + Platt, chosen
per horizon). The full enhancement stacked four things: **+20 engineered features**, a **cross-validated
survival ensemble** (XGBoost Cox PH + Random Survival Forest + Gradient Boosted Survival Trees),
**Optuna** hyperparameter tuning, and the calibration step.

**My role:** modeling, enhancement, and reproducibility — one of three teammates who each contributed
across the pipeline. The repository is engineered for reproducibility: a reusable `src/` package, a
narrative walkthrough notebook and a self-contained Kaggle notebook both generated from the same source,
and figures regenerated directly from the scoring submission.

*(Full methodology, ablations, and exact reproduction steps are in the project repository linked above.)*

---

## Skills Demonstrated

A map from skills to the notebooks that best evidence them:

| Skill area | Representative work |
|---|---|
| **Python / NumPy / pandas** | Unit 1 practice notebooks (vectorization, broadcasting, DataFrame manipulation) |
| **Data cleaning & feature engineering** | Unit 2 — missing data, outliers, one-hot encoding, balanced datasets |
| **Exploratory data analysis & visualization** | Unit 2 — Seaborn/Matplotlib, bivariate plotting, summary statistics |
| **Supervised learning (classification)** | Units 3–4 — KNN, Decision Trees, Logistic Regression |
| **Regression** | Unit 4 (linear regression), Unit 6 (regression model comparison) |
| **Model evaluation & selection** | Unit 5 — cross-validation, confusion matrices, feature selection, model selection |
| **Ensemble methods** | Unit 6 — Random Forests, Gradient Boosted Decision Trees |
| **Unsupervised learning** | Unit 6 — clustering |
| **Deep learning (Keras/TensorFlow)** | Unit 7 — neural networks and CNNs |
| **Natural language processing** | Unit 8 — text features, word embeddings, sentiment analysis |
| **Responsible / fair ML** | Unit 9 — fairness metrics and accountability |
| **Transfer learning & foundation models** | Ursa Space project — ViT / ConvNeXT embeddings |
| **Survival analysis** | WiDS Datathon — Cox PH, Random Survival Forest, Gradient Boosted Survival Trees on right-censored data |
| **Probability calibration** | WiDS Datathon — per-horizon isotonic regression & Platt scaling |
| **Hyperparameter optimization & ensembling** | WiDS Datathon — Optuna (TPE) tuning, cross-validated ensemble weighting |
| **Team collaboration & reproducibility** | Ursa Space & WiDS projects; reproducible `src/` pipeline; Git workflow across repos |

---

## Repository Structure

```
break-through-tech-ai/
├── README.md                     ← you are here (portfolio landing page)
├── LICENSE                       ← MIT license (covers my own code)
├── requirements.txt              ← Python environment for the notebooks
├── .gitignore
├── data/
│   └── README.md                 ← datasets used and where to obtain them
│
├── unit-01-ml-in-a-nutshell/
│   ├── README.md
│   ├── labs/
│   └── practice/
├── unit-02-managing-data/
│   ├── README.md
│   ├── labs/
│   ├── assignments/
│   └── practice/
├── unit-03-common-models-knn-and-trees/
├── unit-04-linear-models/
├── unit-05-evaluation-and-deployment/
├── unit-06-ensembles-and-unsupervised/
├── unit-07-deep-learning-and-computer-vision/
├── unit-08-nlp-and-capstone/
├── unit-09-responsible-ml/
│   └── README.md                 ← theory unit (summary, no notebooks)
│
└── ai-studio-fall-2025-ursa-space/   ← Phase 2: my Ursa Space team-project notebooks
    ├── README.md                 ← project context + my specific contribution
    └── notebooks/
```

Every unit folder has its own `README.md` indexing that unit's notebooks with one-line
descriptions, so you can navigate straight to whatever interests you.

---

## Reproducing This Work

These notebooks were originally run on Cornell Tech's JupyterHub environment. To run them
locally:

**1. Clone the repository**
```bash
git clone https://github.com/Colin-J-Emmanuel/break-through-tech-ai.git
cd break-through-tech-ai
```

**2. Create an environment and install dependencies**
```bash
python3 -m venv .venv
source .venv/bin/activate        # on Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

**3. Get the datasets**
The datasets are **not** committed to this repository. See **[`data/README.md`](./data/README.md)**
for the full list of datasets each notebook uses and where to obtain them (most are standard
public datasets such as Iris, the World Happiness Report, and the Census/Adult income data).

**4. Launch Jupyter**
```bash
jupyter lab
```

> **Tip:** the notebooks are committed **with their outputs intact**, so you can read every
> result, chart, and metric directly on GitHub without running a single cell.

---

## A Note on Course Materials & Academic Integrity

This repository contains **my own completed notebooks** — the work I produced during the
program. Break Through Tech AI is explicitly a portfolio-building program, and showcasing
completed coursework is encouraged.

To respect intellectual property, this repository **deliberately excludes** the program's
proprietary instructional materials — course transcripts, glossaries, toolkit cheat sheets,
and assignment/answer PDFs authored by Cornell Tech / Break Through Tech. Those belong to the
program and are not mine to redistribute. Only my own notebook solutions are published here.

If you are a current fellow: please use this portfolio for reference and inspiration, not as
a shortcut around doing the work yourself — the learning is the point.

---

## About Me

I'm **Colin Emmanuel**, an AI/ML Fellow with Break Through Tech AI at Cornell Tech, interested
in applied machine learning across computer vision, NLP, and real-world data problems.

- **GitHub:** [@Colin-J-Emmanuel](https://github.com/Colin-J-Emmanuel)

---

## Acknowledgements

Thank you to **Break Through Tech** and **Cornell Tech** for the Machine Learning Foundations
curriculum, and to the instructors, coaches, and challenge advisors who supported each AI
Studio. Team acknowledgements for the industry projects appear in their respective repositories.

---

## License

The code and notebooks I authored in this repository are released under the
**[MIT License](./LICENSE)**. Datasets and any third-party materials referenced remain under
their own respective licenses.