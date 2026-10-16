# Regression Challenge 🚀

Hello Class!  

Welcome to the **Regression Challenge**, where you get the chance to apply your machine learning skills to predict **future supermarket sales**! This project is designed to challenge your problem-solving abilities and sharpen your data science toolkit.  

The students with the best scores will earn the spotlight! You’ll be invited to present your solution in class and share your insights.  

---

## 🔍 What’s the Goal?  

Your goal is to predict the column **Quantity_Sold_(kilo)** for a dataset of supermarket sales.  
You’ll be working with real-world data that we deliberately “messed up” — so careful preprocessing and smart feature engineering will be crucial for success.  

---

## 🗂 Files Overview  

You’ll be working with three key files:  

- **unlabeled_data.csv**: Contains ~30% of the dataset, but without the column **Quantity_Sold_(kilo)**.  
  → Your task: predict this column using models such as Linear Regression, Decision Trees, Random Forests, or XGBoost. You can use any model you want as long as you understand it, even if we have not covered it in class yet. 🔮  

- **labeled_data.csv**: Use this dataset to train your model(s). The column **Quantity_Sold_(kilo)** is available here.  

- **example_prediction.csv**: Shows the required format for your final submission, including the **ID** column (from *unlabeled_data.csv*) and a placeholder **Quantity_Sold_(kilo)** column (set to -1).  
  → Your final predictions must match this structure, with one prediction for each ID in *unlabeled_data.csv*.

---

## Steps by Step  

1. **📊 Preprocess the Datasets**  
   - Load both *labeled_data.csv* and *unlabeled_data.csv*.  
   - Split *labeled_data.csv* into training and validation sets.  
   - Handle missing values, outliers, and normalize/standardize if needed.  
   - Clean the dataset and perform feature engineering.
   - Encode categorical variables (e.g., One-Hot or Target Encoding).  

2. **🧠 Train Your Model**  
   - Train machine learning models of your choice (e.g., Linear Regression, Ridge/Lasso Regression, Decision Trees, Random Forests, LightGBM, XGBoost, ...) to predict  **Quantity_Sold_(kilo)** with traindata from labeled_data.csv.
   - Evaluate performance on validationdata from labeled_data.csv  
   - Feel free to explore algorithms we haven’t covered in class yet.  

3. **📈 Prepare Your Predictions**  
   - Apply your best model trained on traindata from labeled_data.csv to *unlabeled_data.csv* to predict the column **Quantity_Sold_(kilo)**.  
   - Save your output in the same format as *example_prediction.csv*.  

4. **📑 Follow the Structure**  
   - **ID Column**: Must be 100% identical to the ID column in *unlabeled_data.csv*.  
   - **Quantity_Sold_(kilo)**: Replace placeholder (-1) values with your actual predictions.  

5. **📤 Upload Your File**  
   - Once ready, upload your prediction file for evaluation here:  
     👉 https://redi-ml-regression-challenge.streamlit.app
   - If you see an error, you most likely don’t have a prediction for every ID in *unlabeled_data.csv*.  
   - You can upload as many solutions as you want.  
   - Submissions will be evaluated using the **Mean Squared Error (MSE)**.  
     - MSE is always non-negative.  
     - **Lower is better** (closer to 0 = more accurate predictions).  

---

## ⚙️ Evaluation Code  

Here’s the snippet we’ll use for scoring:  

```python
from sklearn.metrics import mean_squared_error

# Unknown true values
Y_true = [6.841, 7.356, 1.909, 12.086, ...]  

# Your predictions from uploaded CSV
Y_pred = [0.592, 8.937, 1.993, 11.942, ...]  

# Calculate Mean Squared Error (MSE)
your_score = mean_squared_error(Y_true, Y_pred)  # MSE ≥ 0; closer to 0 is better
```
---
### 🏁 Homework Deadline:  20.10.2026 23:59 (Tuesday)
- Upload at least one prediction to the [website](https://redi-ml-regression-challenge.streamlit.app).

### 🏁 Challenge Deadline: 25.10.2026 23:59 (Sunday)
- The best-performing student will earn honor and recognition 🎉 
---

## 🛠 Teamwork

You want to work in a group? Feel free to share ideas and help with problems, but everyone should write there own code.

---

## 🛠 Resources

- You may use any machine learning method.
- Questions? Stuck? Post in the Slack group chat so everyone can benefit from the answers.
- Please avoid sending private messages to teachers about the challenge.

Have fun exploring the data and training your models! 💪🎉
