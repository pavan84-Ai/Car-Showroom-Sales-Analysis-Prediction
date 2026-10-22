# 🚗 Car Showroom Sales Analysis & Price Prediction

An end-to-end Data Science and Machine Learning project developed as part of an internship assignment. 
This project analyzes car showroom sales data, extracts key business insights regarding customer preferences and showroom performance, 
and builds a robust supervised machine learning pipeline to predict vehicle selling prices.

---

## 📌 Project Overview & Objectives
The management required data-driven answers to core business questions regarding inventory turnover, margin optimization, and pricing accuracy:
1. Which car brands generate the highest sales volume?
2. Which car models are most popular among customers?
3. Which fuel and transmission types dominate the market?
4. How do sales and profitability fluctuate across months and sales personnel?
5. Can we accurately predict a car's selling price using Machine Learning regression algorithms?

---

## 📂 Project Structure & Deliverables
```text
📦 Car-Showroom-Sales-Analysis-Prediction
├── 📜 Car_Showroom_Sales_Analysis_and_Prediction.ipynb  # Complete Python Jupyter Notebook
├── 📊 cleaned_car_showroom_data.csv                    # Sanitized dataset (600 records)
├── 📊 car_showroom_data_raw.csv                          # Raw generated dataset
├── 🤖 car_price_prediction_model.joblib                # Serialized best-performing ML model
├── 📑 Car_Showroom_Sales_Analysis_&_Price_Prediction.pdf # Final formal project report
└── 📊 README.md                                          # Project documentation



---

## 🛠️ Tools & Technologies Used
- **Python** (Programming Language)
- **Pandas & NumPy** (Data Manipulation & Numerical Operations)
- **Matplotlib & Seaborn** (Data Visualization & EDA Plots)
- **Scikit-learn** (Machine Learning Model Training, Pipelines & Evaluation)
- **Google Colab / Jupyter Notebook** (Development Environment)

---

## 📈 Key Exploratory Data Analysis (EDA) Insights
- **Total Performance:** Analyzed 600 vehicle transactions, generating ₹1.00B+ in revenue and ₹129.8M in gross profit.
- **Top Brands:** Toyota (110 units), Honda (106 units), and Maruti Suzuki (103 units) capture over 53% of total unit sales.
- **Top Models:** Toyota Innova, Hyundai Creta, and Honda Amaze lead customer demand.
- **Fuel Preferences:** Petrol leads at 50.3%, followed by Diesel (29.8%), CNG (16.3%), and Electric (3.5%).
- **Profitability by Category:** SUVs and Hatchbacks drive nearly 90% of overall business profits (₹58.8M and ₹58.0M respectively).
- **Seasonality:** Sales peak significantly in June (66 units) with a seasonal dip observed in August.

---

## 🤖 Machine Learning Model Benchmarking
Three supervised regression models were trained using an 80-20 train-test split via scikit-learn Pipelines (incorporating OneHotEncoder to prevent data leakage):

| Model | MAE (₹) | MSE | RMSE (₹) | $R^2$ Score |
| :--- | :---: | :---: | :---: | :---: |
| **Linear Regression** | ₹48,212.26 | 3,851,326,505.73 | ₹62,059.06 | 0.9923 |
| **Random Forest Regressor** | ₹51,079.18 | 4,519,761,382.85 | ₹67,229.17 | 0.9909 |
| **Decision Tree Regressor** | ₹63,825.79 | 7,277,004,672.14 | ₹85,305.36 | 0.9854 |

- **Selected Model:** Linear Regression achieved the highest explained variance ($R^2 = 99.23\%$) and lowest average error margin, making it the optimal lightweight model for deployment.

---

## 💼 Strategic Business Recommendations
1. **Inventory Procurement:** Increase stock allocation for top-performing models like the Toyota Innova and Hyundai Creta.
2. **Monsoon Marketing:** Launch targeted promotional discounts during July and August to counteract seasonal sales slumps.
3. **Automated Trade-In Pricing:** Integrate the serialized `car_price_prediction_model.joblib` into showroom CRM software to provide sales associates with instant, data-backed vehicle valuations.

---

## 👤 Author
- **Pratik Kalavikatte** (Data Analytics Intern)
