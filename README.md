
## 📖 Project Overview
This project is a **Calorie Prediction Model** that estimates the number of calories burned based on user input such as age, weight, heart rate, duration, and body temperature. We use **Machine Learning (XGBoost, SVR, Random Forest)** for predictions and **FastAPI** to serve the model as a web app. The frontend is beautifully designed with a modern **glassmorphism UI** and animated elements for an engaging user experience.

---

## 📊 Dataset Description
The dataset consists of various biometric and exercise-related features that influence calorie burn.

### Features:
- **Gender** (1 = Male, 0 = Female)
- **Age** (years)
- **Height** (cm)
- **Weight** (kg)
- **Duration** (minutes spent exercising)
- **Heart Rate** (bpm - beats per minute)
- **Body Temperature** (°C)
- **Calories** (Target Variable: Energy burned)

### Data Preprocessing:
- Applied feature scaling using **StandardScaler**
- Encoded categorical variables (Gender)

---

## 🚀 Model Training
To find the best-performing model, I trained three models:
1️⃣ **Support Vector Regressor (SVR)**  
2️⃣ **Random Forest Regressor (RFR)**  
3️⃣ **XGBoost Regressor** ✅ (Best Model)


🚀 **XGBoost** outperformed the other models so It was chosen for deployment.

---

## ⚡ FastAPI Deployment
After selecting the XGBoost model, I built a **FastAPI application** to serve predictions.

### 🛠 Steps in Deployment:
1️⃣ Preprocessed user input and scaled it using **StandardScaler**.  
2️⃣ Loaded the trained XGBoost model and applied it to predict calories.  
3️⃣ Created a FastAPI server to handle **POST requests** and return predictions.  
4️⃣ Designed an **elegant UI** with **animated transitions** for user interaction.

---

## 🎨 Frontend Design
The frontend features a **modern glassmorphism design** with smooth animations for a delightful user experience. Key design elements include:
- **Animated input fields** that expand on focus.
- **Interactive buttons** with hover effects.
- **Dynamic result display** with fade-in animations.

---

## 🧪 Test Set Performance
The final XGBoost model was rigorously tested, achieving outstanding results:

| Metric       | Test Set Performance |
|--------------|----------------------|
| **R² Score** | **0.9991**           |
| **MAE**      | **1.260**            |
| **RMSE**     | **1.892**            |

These metrics confirm the model's **exceptional generalization** and **high accuracy**.

---

## 🛠️ Tech Stack
- **Machine Learning**: XGBoost, SVR, Random Forest
- **Backend**: FastAPI
- **Frontend**: HTML, CSS, JavaScript (with animations)
- **Data Preprocessing**: Pandas, Scikit-learn
- **Deployment**: Docker, Uvicorn

---

