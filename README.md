# 📊 Telecom Customer Churn Prediction

This project focuses on predicting customer churn in the telecom industry using machine learning techniques. Churn prediction helps identify at-risk customers, allowing companies to implement retention strategies proactively.

---

## 🧠 **Problem Overview**

Telecom companies face high customer acquisition costs, making customer retention a key priority. Using historical customer data, this project aims to:

* Understand which features correlate most with customer churn.
* Train machine learning models to predict churn.
* Deliver actionable insights to reduce churn rates.

---

## 🔁 **Workflow Summary**

1. **Data Preprocessing**

   * Converted object types to categorical/numerical.
   * Handled missing values by filling NaNs appropriately.
   * Removed duplicates and encoded categorical variables.

2. **Exploratory Data Analysis (EDA)**

   * Analyzed churn distribution and visualized it with pie charts.
   * Explored the impact of monthly charges, tenure, age, and contract type on churn through group-by operations and bar charts.
   * Displayed histograms for numerical distributions like Monthly Charges and Tenure.

3. **Feature Engineering**

   * Encoded categorical features like `Gender` and `Churn` into numerical values.
   * Scaled continuous variables with `StandardScaler`.

4. **Modeling**

   * Implemented five classification models:

     * Logistic Regression
     * Random Forest
     * Support Vector Machine (Best Performing)
     * K-Nearest Neighbors
     * Decision Tree
   * GridSearchCV was used for hyperparameter tuning.

5. **Model Evaluation**

   * Evaluated models using Accuracy, Precision, and Recall.
   * Used Confusion Matrix and ROC-AUC Curve to analyze model performance.

---

## 🧰 **Tech Stack**

* **Python**
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn, Streamlit

---

## ✨ **Key Insights**

* Month-to-month contracts have the highest churn risk.
* Customers with fiber optic internet and no tech support are more likely to churn.
* Tenure and contract type are strong predictors.

---

## 🚀 **Streamlit App**

The application allows users to:

* Input customer details such as Age, Gender, Tenure, and Monthly Charges.
* Predict the likelihood of a customer churning.

### **App Features:**

* Real-time predictions.
* Interactive user interface.
* Display of churn probability.

!\[Streamlit Dashboard Screenshot]\(./Streamlit Application.png)

---

## 📂 **Project Structure**

```
📦customer-churn-prediction
 ┣ 📜app.py
 ┣ 📜customer_churn_data.csv
 ┣ 📜model.pkl
 ┣ 📜notebook.ipynb
 ┣ 📜scaler.pkl
 ┗ 📜Streamlit Application.png
```

---

## **Setup Instructions**

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/customer-churn-prediction.git
   ```

2. Navigate to the project directory:

   ```bash
   cd customer-churn-prediction
   ```

3. Create and activate a virtual environment:

   ```bash
   python3 -m venv venv
   source venv/bin/activate    # For Linux/Mac
   .\venv\Scripts\activate   # For Windows
   ```

4. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

5. Run the Streamlit app:

   ```bash
   streamlit run app.py
   ```

6. Access the application at `http://localhost:8501`

---

## **References**

* [Streamlit Documentation](https://docs.streamlit.io/)
* [Scikit-Learn Documentation](https://scikit-learn.org/stable/documentation.html)

Feel free to contribute to this project by creating pull requests, reporting issues, or suggesting features.

---

## **Author:**

Jay
