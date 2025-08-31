# Online Review Quality Filter

## Project Overview
This project is designed to automatically detect and filter low-quality online reviews, including spam, advertisements, irrelevant content, and misleading rants. The goal is to improve the reliability of online review data for both users and platforms.  

The project includes:  
- **Feature Engineering & Baseline Models:** Text preprocessing, embeddings, and traditional ML models (Logistic Regression, SVM) to establish a baseline.  
- **Fine-Tuned Language Model:** A small variant of Gemini/Qwen, fine-tuned locally for review classification.  
- **Rule-Based Policy Module:** Optional rules to catch extreme cases or policy-specific violations.  

This workflow allows users to classify reviews effectively and experiment with improving model performance.

---

## Repository Structure
```text
├── notebooks/
├── pipeline/
│ ├── feature_engineering_and_baseline.ipynb
│ ├── fine_tuning_model.ipynb
│ └── rule_based_policy_module.ipynb
├── models/
│ ├── logreg_model.joblib
│ ├── numeric_scaler.joblib
│ ├── svm_model.joblib
│ └── tfidf_vectorizor.joblib
├── documents/ # some files
├── data/ # containing datasets
└── README.md
```
The folder **pipeline** contains all the notebooks used for this project, and **models** contains the saved components for baseline models. Note that for the fine-tuned model, the model components are too large to be uploaded to github. Therefore they are not included here.

## Setup Instructions
1. **Download the Notebooks:**  
   - Download the notebooks from this repository to your own environment (local machine or preferred IDE).

2. **Adjust File Paths:**  
   - All the notebooks use Google Drive mounting. After downloading to your personal environment, you can delete it or replace it with the file paths on your local computer.  
   - for **Data_Preprocessing.ipynb**, **do not need to re-run** the notebook as the output has already been saved as separate data files. Please refer to the section **Pseudo Ground-truth Labelling** for the algorithm for ground-truth labeling and related results.
   - The **Feature_Engineering_and_Model.ipynb** contains the baseline models (SVM and Logistic regression). Please refer to the beginning of the notebook for user guide.
   - Similar for the **FineTuning.ipynb**, please refer to the beginning of the notebook for detailed user guide
