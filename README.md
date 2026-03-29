# 🍔 Food Delivery Time Estimation 🚴‍♂️

## 📌 Project Overview

This project focuses on predicting food delivery time using machine learning techniques. The dataset includes information about delivery personnel, restaurant and delivery locations, weather conditions, traffic density, and more.

The goal is to build an accurate predictive model that estimates delivery time based on real-world factors.

---

## 📂 Dataset Description

The dataset consists of two files:

* `train.csv` → used for training the model
* `test.csv` → used for predictions

### 🧾 Features

| Column Name                            | Description                     |
| -------------------------------------- | ------------------------------- |
| ID                                     | Unique order ID                 |
| Delivery_person_ID                     | ID of delivery agent            |
| Delivery_person_Age                    | Age of delivery person          |
| Delivery_person_Ratings                | Ratings of delivery person      |
| Restaurant_latitude / longitude        | Restaurant location             |
| Delivery_location_latitude / longitude | Delivery location               |
| Order_Date                             | Date of order                   |
| Time_Orderd                            | Order time                      |
| Time_Order_picked                      | Pickup time                     |
| Weatherconditions                      | Weather during delivery         |
| Road_traffic_density                   | Traffic level                   |
| Vehicle_condition                      | Condition of delivery vehicle   |
| Type_of_order                          | Category of order               |
| Type_of_vehicle                        | Vehicle used                    |
| multiple_deliveries                    | Number of deliveries handled    |
| Festival                               | Festival indicator              |
| City                                   | City type                       |
| Time_taken(min)                        | Target variable (delivery time) |

---

## 🧹 Data Preprocessing

* Handled missing values and inconsistent entries
* Converted date and time columns into useful features
* Cleaned target variable (`Time_taken(min)`)
* Removed duplicates
* Encoded categorical variables
* Created new features such as:

  * Distance between restaurant and delivery location
  * Order preparation time
  * Time-based features (hour, weekday, etc.)

---

## 📊 Exploratory Data Analysis (EDA)

Performed visual and statistical analysis:

* Distribution plots (histograms)
* Box plots for outlier detection
* Scatter plots for relationships
* Correlation heatmap

---

## 🧠 Feature Engineering

Key engineered features:

* 📍 Distance using Haversine formula
* ⏱ Preparation time (order to pickup)
* 📅 Date-based features (day, month, weekday)
* 🕒 Time-based features (hour of order/pickup)

---

## 🤖 Machine Learning Model

Used:

* 🌲 Random Forest Regressor

Other models can be explored:

* XGBoost
* LightGBM
* Linear Regression

---

## 📈 Model Evaluation

Metrics used:

* R² Score
* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)

---

## 🚀 Results

The model successfully predicts delivery time with reasonable accuracy by leveraging spatial, temporal, and environmental factors.

---

## 🛠 Tech Stack

* Python 🐍
* Pandas & NumPy
* Matplotlib & Seaborn
* Scikit-learn

---

## 📌 Future Improvements

* Hyperparameter tuning
* Advanced models (XGBoost, Deep Learning)
* Real-time prediction system
* Deployment using Flask/Streamlit

---

## ▶️ How to Run

```bash
# Clone repository
git clone https://github.com/your-username/food-delivery-time

# Install dependencies
pip install -r requirements.txt

# Run notebook/script
python main.py
```

---

## 🙌 Conclusion

This project demonstrates how machine learning can be applied to optimize logistics and improve delivery efficiency in real-world scenarios.

---

## ⭐ If you like this project

Give it a ⭐ on GitHub!
