# Distributed Hyperparameter Tuning for Random Forests using Ray Tune

This repository showcases a scalable approach to hyperparameter tuning for a `RandomForestClassifier` using **Ray Tune** and a **Grid Search** strategy. The task involves predicting forest cover types using the **Covertype** dataset.

---

## 🚀 Project Overview

Hyperparameter tuning is essential for optimizing machine learning models. However, it's often computationally expensive. In this project, we transform the tuning process into a **task-parallel workflow** using **Ray Tune**, allowing the execution of multiple training jobs in parallel across multiple VMs.

---

## 📊 Problem Statement
Train a `RandomForestClassifier` on the **Covertype dataset** and optimize the following hyperparameters:

- `max_depth`
- `n_estimators`
- `ccp_alpha`

### Dataset:
- Source: `sklearn.datasets.fetch_covtype`
- Description: Forest Cover Type Prediction dataset

---

## 🧰 Tools & Technologies
- Python 3.x
- scikit-learn
- Ray Tune
- Grid Search
- Distributed computing (tested on up to 3 small VMs)

---

## 📂 Repository Structure
```
├── notebooks/                  # Jupyter notebooks for data exploration and training
├── scripts/                    # Python scripts for training and tuning
├── requirements.txt            # Python dependencies
└── README.md                   # Project documentation
```

---

## ⚙️ Setup & Installation
1. Clone the repository:
```bash
git clone https://github.com/your-username/rf-raytune-hyperparam.git
cd rf-raytune-hyperparam
```

2. Create and activate a virtual environment:
```bash
python3 -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

4. Run the training script (example):
```bash
python scripts/tune_random_forest.py
```

---

## 📈 Results
The project runs an exhaustive grid search across specified hyperparameter ranges using Ray Tune. Results are logged and analyzed to select the optimal configuration based on accuracy.

---

## 📎 References
- [Scikit-learn RandomForestClassifier Documentation](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)
- [Ray Tune Documentation](https://docs.ray.io/en/latest/tune/index.html)
- [Covertype Dataset on Kaggle](https://www.kaggle.com/competitions/forest-cover-type-prediction)

---

## 📬 Contact
For questions or contributions, feel free to open an issue or reach out via GitHub.
