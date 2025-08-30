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
│ ├── feature_engineering_and_baseline.ipynb
│ ├── fine_tuning_model.ipynb
│ └── rule_based_policy_module.ipynb
├── documents/ # some files
├── data/ # containing datasets
└── README.md
```


## Setup Instructions
1. **Download the Notebooks:**  
   - Download the notebooks from this repository to your own environment (local machine or preferred IDE).

2. **Adjust File Paths:**  
   - If the notebooks use Google Drive mounting, replace it with the file paths on your local computer.  
   - Make sure your dataset and any required files are correctly referenced.
