# 🧠 Predicting Mental Health Severity from Digital Habits

### 📌 Project Overview
With the increasing dependency on digital devices, this project investigates whether daily screen time and lifestyle habits (sleep, physical activity) can accurately predict the severity of mental health issues. Using a dataset of ~2,000 participants, we applied Machine Learning techniques to classify individuals into "Normal" or "Severe" risk categories.

### 🚀 Key Problem & Solution
* **The Challenge:** Real-world health data is often imbalanced. In our dataset, "Severe" cases were the minority, causing standard models to ignore them (High Accuracy, but near-zero Recall).
* **The Solution:** We implemented **CTGAN (Conditional Tabular GAN)**, a Generative AI technique, to generate synthetic data and balance the classes.

### 🛠️ Tech Stack
* **Language:** Python
* **Libraries:** Pandas, Scikit-Learn, XGBoost, Imbalanced-learn (SMOTE), SDV (CTGAN)
* **Visualization:** Matplotlib, Seaborn

### 📊 Key Findings
1.  **Screen Time isn't the only factor:** Correlation analysis showed that screen time alone had a weak linear relationship with mental health scores; it is the *combination* of sleep, activity, and digital habits that matters.
2.  **The Accuracy Trap:** Standard Random Forest models achieved ~76% accuracy but failed to detect severe cases (Recall: 7%).
3.  **GenAI Impact:** Training Logistic Regression on **CTGAN-augmented data** significantly improved the Recall (Sensitivity) for the "Severe" class, jumping from ~17% to nearly 49%, making the model much more useful for screening purposes.

### 📂 Files in this Repository
* `Mental_Health_Analysis.html`: The full code and visualizations.
* `Final_Report.pdf`: Detailed academic report covering methodology and literature review.
* `Project_Poster.pdf`: A visual summary of the project flow and results.

---
*This project was completed as part of the HDS-5960 Capstone at Saint Louis University.*
