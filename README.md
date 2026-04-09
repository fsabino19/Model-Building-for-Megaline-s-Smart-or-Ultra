# TripleTen Sprint 7 Project – Machine Learning: Plan Recommendation

This is one of the core machine learning projects I completed in the TripleTen Data Science program. It was my first full end‑to‑end modeling task, where I trained and evaluated multiple algorithms to help a mobile carrier improve their plan recommendation system.

---

# Megaline Plan Recommendation

Megaline, a mobile carrier, discovered that many subscribers still use outdated legacy plans. They want to transition customers to one of their newer offerings — **Smart** or **Ultra** — and need a model that can analyze user behavior and recommend the most suitable plan.

The goal of the project was to build a **classification model** that predicts whether a subscriber should be recommended the Smart plan or the Ultra plan based on their monthly usage patterns.

---

# The Data

The dataset contains subscriber behavior over a one‑month period. Each row represents one user and includes their usage metrics along with the plan they ultimately chose.

The data was provided by TripleTen.

### Columns

- **calls** — number of calls the user made during the month  
- **minutes** — total minutes spent on calls  
- **messages** — number of text messages sent  
- **mb_used** — total mobile data used (in megabytes)  
- **is_ultra** — target variable:  
  - `1` → Ultra plan  
  - `0` → Smart plan  

---

# The Process

### 1. Data Exploration
- Reviewed distributions, checked for anomalies, and validated data types.  
- Confirmed there were no missing values or duplicates.

### 2. Train/Validation/Test Split
- Split the dataset into training, validation, and test sets to ensure reliable evaluation.

### 3. Model Training
I trained and tuned several models, including:
- Decision Tree Classifier  
- Random Forest Classifier  
- Logistic Regression  

Hyperparameters were tuned using validation accuracy to identify the best‑performing model.

### 4. Model Evaluation
- Compared models using validation accuracy.  
- Selected the model with the strongest generalization performance.  
- Performed a final evaluation on the test set to confirm stability.

### 5. Sanity Check
Ensured the model wasn’t overfitting and behaved logically across different usage patterns.

---

# Results

The best model achieved strong accuracy on both the validation and test sets, meeting the project requirement of **≥ 0.75 accuracy**.

The model successfully learned patterns in call duration, message volume, and data usage to distinguish between Smart and Ultra plan users.

This project strengthened my understanding of:
- Model selection  
- Hyperparameter tuning  
- Avoiding overfitting  
- Evaluating classification performance  
- Communicating machine learning results clearly  

Please refer to the Jupyter Notebook in this repository for the full workflow, code, and analysis.
