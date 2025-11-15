# 📉 Employee Attrition Prediction using Machine Learning

## Project Goal
Developed a robust **Machine Learning (ML) classification model** to proactively predict which employees are at high risk of leaving the company (**attrition**). This project demonstrates the ability to build and test **AI/ML models** and deliver **data-driven insights** for business strategy.

## 🛠️ Technologies & Tools
This project utilized **Core Python** and the core stack for data science and ML, aligning with the Netlink JD requirements:

* **Core Python**
* **AI/ML:** Scikit-learn (Model Training, Hyperparameter Tuning, Evaluation)
* **Data Analysis:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn

## 🚀 Key Results & Performance
The **Random Forest Classifier** was selected as the final model for its high predictive accuracy and strong feature importance extraction on the imbalanced dataset.

| Metric | Result (*Update with your actual values from the notebook*) |
| :--- | :--- |
| **Final Model** | Random Forest Classifier |
| **Accuracy** | [90.5%] |
| **Precision (Attrition Class)** | [78%] |
| **Recall (Attrition Class)** | [70%] |
| **F1 Score (Attrition Class)** | [73.8%] |

---

## ⚙️ Methodology & Skills Demonstrated

### 1. Data Cleaning and EDA
* Loaded and prepared the **IBM HR Analytics Employee Attrition Dataset**.
* Performed **Exploratory Data Analysis (EDA)** using Matplotlib and Seaborn to visualize feature distributions and identify patterns associated with high attrition.
* Cleaned data by dropping constant/irrelevant identifiers (`EmployeeCount`, `StandardHours`) and handling missing values to maintain model focus and efficiency.

### 2. Data Preprocessing and Feature Engineering
* Applied **One-Hot Encoding** (using Pandas `get_dummies()`) to convert nominal categorical features (e.g., `Department`, `MaritalStatus`) into numerical format.
* Used **Label Encoding** for ordinal features (e.g., `Education`, `JobLevel`).
* Scaled numerical features using `StandardScaler` to prevent feature dominance and optimize model performance.
* Addressed the target variable's class imbalance (high No-Attrition vs. low Attrition) to ensure robust model training.

### 3. Model Development and Evaluation
* Split the dataset into training and testing sets (e.g., 80/20) for rigorous **testing and validation**.
* Trained and evaluated several classification algorithms (**Logistic Regression, Random Forest**) using Scikit-learn.
* Optimized the final model using **Hyperparameter Tuning** to achieve the reported performance metrics.
* Model was evaluated based on the **Confusion Matrix**, **Precision**, and **Recall** (crucial for attrition prediction).

---

## 📊 Key Business Insights

Feature Importance analysis derived from the Random Forest model revealed the most influential predictors of employee attrition, enabling proactive, **data-driven decision making**.

* **OverTime:** Employees working **Overtime** were one of the strongest indicators of attrition risk.
* **Monthly Income & Job Level:** Lower income levels and lower Job Levels correlated strongly with higher attrition.
* **Job Satisfaction:** Employees with lower Job Satisfaction and poor Work-Life Balance scores showed a higher likelihood of leaving.

This predictive model provides HR management with the necessary insights to intervene with targeted retention strategies (e.g., compensation review, workload adjustment).

---
*The full analysis and code walkthrough is available in the **`Employee Attrition Notebook.ipynb`**.*
