# ⚡ Fitness & Calorie Burn Predictor

A Machine Learning web application that predicts total calories burned during a workout session based on user demographics and physiological metrics. Built with **Scikit-Learn**, **Pandas**, and **Streamlit**.

---

## 📌 Features

- **Personalized Predictions:** Input user details (Age, Gender, Height, Weight) and activity metrics (Duration, Heart Rate, Body Temp) to calculate total calorie expenditure[cite: 1, 2].
- **Automated Preprocessing:** Utilizes a Scikit-Learn `Pipeline` with `StandardScaler` and `OneHotEncoder`.
- **BMI Metrics:** Displays real-time Body Mass Index (BMI) along with health classification.
- **Interactive Web UI:** Clean, intuitive interface powered by Streamlit.

---

## 📊 Dataset & Features

The model is trained on workout and physiological data using the following attributes:

- **Features (`X`)**:
  - `Age`: Age in years[cite: 1, 2]
  - `Gender`: Male / Female[cite: 1, 2]
  - `Height`: Height in centimeters[cite: 1, 2]
  - `Weight`: Weight in kilograms[cite: 1, 2]
  - `Duration`: Workout duration in minutes[cite: 1, 2]
  - `Heart_Rate`: Average heart rate during workout (bpm)[cite: 1, 2]
  - `Body_Temp`: Body temperature during workout (°C)[cite: 1, 2]
- **Target (`y`)**:
  - `Calories`: Total calories burned[cite: 2]

---

## ⚙️ Tech Stack

- **Language:** Python
- **Libraries:** Pandas, Scikit-Learn, Pickle[cite: 1, 2]
- **Model:** RandomForestRegressor[cite: 2]
- **Web Framework:** Streamlit

---

## 📁 Repository Structure

```text
├── app.py                # Streamlit web application
├── train_model.py        # Model training and evaluation script
├── calories.csv          # Workout dataset
├── fitness_model.pkl     # Saved Scikit-Learn pipeline (generated after training)
└── README.md             # Project documentation
