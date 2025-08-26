# Titanic Survival Prediction  

This project analyzes the Titanic dataset and builds a **Random Forest Classifier** to predict passenger survival.  
The dataset is one of the most well-known beginner challenges, originally from the **Kaggle Titanic Machine Learning Challenge**.  

---

## Dataset  

- **Source:** [Kaggle - Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic)  
- **Features:**  
  - Passenger details → `Name`, `Sex`, `Age`  
  - Ticket info → `Pclass`, `Fare`, `Cabin`, `Ticket`  
  - Family info → `SibSp`, `Parch`  
  - Boarding → `Embarked`  
- **Target Variable:** `Survived` (1 = Survived, 0 = Did not survive)  

---

## Analysis Performed  

1. **Exploratory Data Analysis (EDA):**  
   - Checked missing values and distributions.  
   - Analyzed survival rates by **gender**, **class**, **age groups**, and **family size**.  

2. **Data Preprocessing:**  
   - Filled missing values (`Age`, `Embarked`).  
   - Converted categorical variables (`Sex`, `Embarked`) into numeric form.  
   - Dropped irrelevant features (`Name`, `Ticket`, `Cabin`).  

3. **Modeling:**  
   - Implemented a **Random Forest Classifier**.  
   - Tuned hyperparameters for better accuracy.  
   - Evaluated using **accuracy, precision, recall, and F1-score**.  

---

## Results  

- **Random Forest Accuracy:** ~79.33%  
- Key Insights:  
  - **Gender (Sex)** was the strongest predictor of survival (females had higher survival rates).  
  - **Passenger class (Pclass)** significantly impacted survival (1st class passengers had better chances).  
  - **Age and family size** also influenced survival probabilities.  

👉 **Random Forest was chosen** because it:  
- Handles both categorical and numerical features well.  
- Reduces overfitting compared to a single Decision Tree.  
- Provides **feature importance**, giving insights into what mattered most for survival.  
