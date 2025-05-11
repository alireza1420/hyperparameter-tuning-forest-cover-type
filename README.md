⚙️ Distributed Hyperparameter Tuning for Random Forests using Ray Tune
This project demonstrates a scalable approach to hyperparameter tuning for a RandomForestClassifier using Ray Tune and Grid Search. The goal is to identify the optimal model configuration for classifying forest cover types based on the Covertype dataset (retrieved via sklearn.datasets.fetch_covtype).

🚀 Key Features
✅ Uses scikit-learn for model training (RandomForestClassifier)

📊 Tunes key hyperparameters: max_depth, n_estimators, and ccp_alpha

🔄 Parallelized grid search using Ray Tune

🖥️ Deployable on a distributed setup with up to 3 small virtual machines

📂 Structured codebase with modular setup for experimentation and evaluation

📚 Background
Hyperparameter tuning is a computationally intensive process crucial for optimizing machine learning models. By leveraging Ray Tune, this project transforms it into a task-parallel workflow, significantly reducing the tuning time by running training jobs in parallel across multiple VMs.

📦 Tools & Frameworks
Python

Scikit-learn

Ray Tune

Grid Search

Distributed Computing with Ray

📝 Getting Started
To run this project, refer to the notebooks/ and scripts/ folders for setup instructions, and requirements.txt for dependencies.

