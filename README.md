
# 📑 Project Overview: Medical Insurance Cost Prediction
In this project, we developed a predictive model to estimate medical insurance expenses using Support Vector Regression (SVR). The goal was to understand how demographic and health factors—such as age, BMI, and smoking status—influence financial risk in the healthcare sector.

### 🔍 1. Exploratory Data Analysis (EDA)
We started by analyzing the distribution of 1,338 observations. Key insights included:

 - The Smoking Gap: Smoking status emerged as the most significant driver of costs.
 - BMI Interaction: For smokers, costs skyrocket exponentially once BMI exceeds 30.
 - Age Correlation: A clear positive trend shows medical expenses rising naturally with age.

### 🛠 2. Data Preprocessing & Engineering
To prepare the data for the SVR model, we performed several critical steps:

 - Categorical Encoding: Converted nominal features (Sex, Smoker, Region) into numerical formats using One-Hot Encoding.
 - Feature Scaling: Applied StandardScaler to numerical features (Age, BMI, Children) to ensure they are on the same scale, which is vital for SVR performance.
 - Target Scaling: Scaled the 'Expenses' variable to improve model convergence during training.

### 🤖 3. Model Development (The Baseline)
We implemented a Support Vector Regression (SVR) model using the RBF kernel.

 - Our initial model achieved an R² of 0.8465, meaning it successfully explained over 84% of the variance in medical costs.
 - The MAE of $2,488 showed that our predictions were reasonably close to actual expenses for the majority of the dataset.

### 🚀 4. Optimization (Advanced Phase)
As an optional but impactful step, we conducted Hyperparameter Tuning via GridSearchCV. 
By fine-tuning C and Gamma, we pushed the model's accuracy further:

 - Improved R²: 0.8573
 - This phase ensured the model was robust against outliers and better at generalizing for new, unseen data.

### 💡 Conclusion
Our analysis confirms that SVR is a powerful tool for insurance cost prediction. By combining rigorous preprocessing with systematic optimization, we created a model that provides reliable financial forecasts, helping insurance providers better understand and mitigate risk.
