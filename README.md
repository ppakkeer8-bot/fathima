#  Customer Purchase Prediction with Interpretable Machine Learning

This project builds a binary classification model to predict **customer purchase behavior** using machine learning techniques. The focus is on **interpretability** with SHAP (SHapley Additive exPlanations), ensuring transparency in how predictions are made.

---

##  Repository Structure
customer-purchase-prediction/ │ ├── data/ │ └── customer_purchase_data.csv # Dataset used for training/testing │ ├── notebooks/ │ └── model_training.ipynb # Jupyter notebook with full workflow │ ├── visuals/ │ ├── shap_summary.png # SHAP global feature importance │ └── confusion_matrix.png # Model evaluation visualization │├── README.md # Project documentation ├── report.pdf # Detailed project report └── requirements.txt # Python dependencies


---

##  Project Workflow

1. **Data Preprocessing**
   - Handled missing values
   - Encoded categorical variables
   - Split dataset into training/testing sets

2. **Model Development**
   - Implemented **Random Forest** and **Gradient Boosting**
   - Optimized hyperparameters using **Grid Search** and **Cross-Validation**

3. **Evaluation**
   - Metrics: Accuracy, Precision, Recall, F1-score
   - Confusion matrix visualization

4. **Interpretability**
   - Applied **SHAP values** for global and local feature importance
   - Compared SHAP with traditional feature importance methods

5. **Documentation**
   - Comprehensive report (`report.pdf`)
   - Visualizations (`visuals/` folder)
   - Annotated notebook (`notebooks/model_training.ipynb`)

---

##  Model Performance (Sample)

| Metric      | Value |
|-------------|-------|
| Accuracy    | 0.87  |
| Precision   | 0.85  |
| Recall      | 0.83  |
| F1-Score    | 0.84  |

---

##  SHAP Insights

- **Global Importance**: Identified top features influencing purchase decisions  
- **Local Explanation**: Visualized individual predictions for transparency  
- **Comparison**: Benchmarked SHAP against traditional feature importance  

---

##  Report

 [View the full report](./report.pdf) for methodology, analysis, and recommendations.

---

##  Getting Started

Clone the repository and install dependencies:

```bash
git clone https://github.com/yourusername/customer-purchase-prediction.git
cd customer-purchase-prediction
pip install -r requirements.txt

Run the notebook:
jupyter notebook notebooks/model_training.ipynb

 Requirements
All dependencies are listed in requirements.txt. Key libraries include:

pandas

numpy

scikit-learn

matplotlib

seaborn

shap

Key Takeaways
Customers with higher engagement and recent activity are more likely to purchase

Age and income levels significantly influence buying behavior

SHAP values provide actionable insights for marketing and policy decisions

Future Work
Add more advanced models (XGBoost, LightGBM)

Extend dataset with additional customer features

Deploy model as an API for real-time predictions

