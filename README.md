# Machine-Learning-IoT-DoS-Detection
The project was submitted in fulfilment of the requirements for the award of the degree of **Master of Science in Cyber Security** at Asia Pacific University of Technology and Innovation.

This repository contains the implementation and deliverables of my Master’s dissertation project, which focuses on developing a lightweight machine learning (ML) framework for detecting Denial-of-Service (DoS) attacks in Internet of Things (IoT) environments.

Using the CICIoT2023 dataset, five ML models were evaluated — Decision Tree, Naïve Bayes, Logistic Regression, Linear Discriminant Analysis (LDA), and Light Gradient Boosting Machine (LGBM). After feature reduction and performance analysis, LGBM emerged as the most robust and efficient model, making it suitable for deployment on resource-constrained IoT devices.

## Deliverables
This project produces the following outputs, all included in this repository:
- 📄 **Thesis Document**: A comprehensive record of the project’s background, methodology, results, and discussion.
- 💻 **Source Code**: Complete ML pipeline in dissertation-project-code.ipynb.
- 🧠 **Saved Model Files**:
  - Models trained on all 20 selected features (dt-20.joblib, lgbm-20.joblib)
  - Models trained on 19 features, excluding the top-ranked feature (dt-19.joblib, lgbm-19.joblib)
- 📊 **Evaluation Results**: A PDF (Collected Results.pdf) containing screenshots of key performance metrics and results. 

## How to Run
> The Python notebook (dissertation-project-code.ipynb) was developed in Kaggle Notebook and should be run in the Kaggle environment.
- Download the Python notebook `dissertation-project-code.ipynb`.
- Upload the notebook to [Kaggle](https://www.kaggle.com/work).
- Open the notebook and click `Run All`.

## Key Highlights
- **Dataset**: CICIoT2023
- **Preprocessing**: Class balancing + dimensionality reduction (41 → 20 features) using Pearson correlation, Mutual Information, and Random Forest feature importance.
- **Evaluation Metrics**: Accuracy, Precision, Recall, F1-score, training/prediction time, and memory usage.
- **Results**: Decision Tree and LGBM achieved near-perfect performance, but LGBM demonstrated superior robustness under feature loss.
