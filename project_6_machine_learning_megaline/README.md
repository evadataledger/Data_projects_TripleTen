# Project 6: Predicting the Right Mobile Plan - Megaline (Machine Learning)

## Objective:

Megaline, a mobile telecom carrier, wants to transition users from legacy plans to their newer offerings - **Smart** and **Ultra**. 
The goal of this project is to develop a **classification model** that predicts which plan a subscriber is likely to choose based on their past monthly behavior. 

## Sucess Metric

- **Accuracy ≥ 0.75** on the test dataset

## Dataset

Each row contains monthly behavior data of one user:
- `calls`: Number of calls
- `minutes`: Total call duration in minutes
- `messages`: Number of text messages
- `mb_used`: Internet traffic used in MB
- `is_ultra`: Target variable (1 = Ultra plan, 0 = Smart plan)

File: `users_behavior.csv`

## Tools & Skills

- Machine Learning (classification)
- Model selection & hyperparameter tuning
- Data splitting (train/valid/test)
- Scikit-learn
- Accuracy metric
- Randomization & validation

## Project Stages

1. **Data Review & Preparation**
   - Verified shape and distribution of features
   - Checked for imbalances and missing values

2. **Model Building**
   - Models tested:
     - Decision Tree
     - Random Forest
     - Logistic Regression
   - Grid search & manual tuning on validation set

3. **Model Evaluation**
   - Measured final model accuracy on test set
   - Compared performance across models

4. **Sanity Checks**
   - Verified reliability by testing model on unseen data
   - Analyzed misclassifications and potential bias

---

## Outcome
- Final model exceeded the 0.75 accuracy threshold.  
- Random Forest was found to be the most reliable in balancing prediction power and stability.  
- Ready for deployment as a plan recommender tool for Megaline’s marketing team.

---

## Folder Structure 

```bash
project_6_machine_learning_megaline/
├── notebooks/
│ └── project_6_machine_learning_megaline.ipynb
├── data/
│ └── users_behavior.csv
├── README.md
├── requirements.txt
