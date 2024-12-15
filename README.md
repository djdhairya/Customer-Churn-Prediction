# Customer Churn Prediction App

## Project Overview

This project predicts customer churn using a **Random Forest Classifier**. Customer churn refers to the likelihood of a customer leaving a service provider. The prediction model utilizes various customer attributes such as demographics, subscription details, and service usage.

A web application built with **Flask** allows users to input customer details and receive predictions along with the probability of churn.

---

## Features

- **Machine Learning**: Random Forest Classifier for churn prediction.
- **Data Preprocessing**: Encoders and scalers for categorical and numerical data transformation.
- **Web Application**: User-friendly interface for predictions.
- **Scalable Design**: Easily adaptable to new features.

---

## Dataset Features

The model uses the following features for prediction:

### Demographics:

- `gender`
- `SeniorCitizen`
- `Partner`
- `Dependents`

### Service Details:

- `PhoneService`
- `MultipleLines`
- `InternetService`
- `OnlineSecurity`
- `OnlineBackup`
- `DeviceProtection`
- `TechSupport`
- `StreamingTV`
- `StreamingMovies`

### Contract Information:

- `Contract`
- `PaperlessBilling`
- `PaymentMethod`

### Subscription Metrics:

- `tenure`
- `MonthlyCharges`
- `TotalCharges`

---

## Requirements

- Required Libraries:
  - Flask
  - pandas
  - scikit-learn
  - pickle
  - matplotlib
  - numpy

---

## How to Run the Application

### 1. Clone the Repository

```bash
git clone 
```

### 2. Start the Flask Server

```bash
python app.py
```

### 3. Access the Application

Open your browser and go to:`http://127.0.0.1:5000/`

---

## Folder Structure

```
|__ data
├── app.py                     
├── model/
│   ├── best_model.pkl         
│   ├── encoder.pkl            
│   ├── scaler.pkl             
├── templates/
│   └── index.html             
── README.md                  
```

---

## Application Flow

1. **Input Data**: User provides customer details in a web form.
2. **Data Preprocessing**:
   - Encodes categorical features.
   - Scales numerical features (`tenure`, `MonthlyCharges`, `TotalCharges`).
3. **Prediction**:
   - Outputs whether the customer is likely to **Churn** or **Not Churn**.
   - Provides the probability of churn.
4. **Output**: Results are displayed on the web interface.

---

## Sample Input

| Feature            | Example Value |
| ------------------ | ------------- |
| `gender`           | Male          |
| `SeniorCitizen`    | 0 (No)        |
| `Partner`          | Yes           |
| `Dependents`       | No            |
| `tenure`           | 24            |
| `PhoneService`     | Yes           |
| `MultipleLines`    | No            |
| `InternetService`  | Fiber optic   |
| `OnlineSecurity`   | No            |
| `OnlineBackup`     | Yes           |
| `DeviceProtection` | No            |
| `TechSupport`      | No            |
| `StreamingTV`      | Yes           |
| `StreamingMovies`  | Yes           |
| `Contract`         | Two year      |
| `PaperlessBilling` | No            |
| `PaymentMethod`    | Credit card   |
| `MonthlyCharges`   | 85.75         |
| `TotalCharges`     | 2075.5        |

---

## Future Enhancements

- Add functionality to train models directly through the app.
- Support additional machine learning models for comparison.
- Deploy the app on cloud platforms like AWS, GCP, or Heroku.
- Improve the user interface for better usability.

---
![Screenshot 2024-12-15 185631](https://github.com/user-attachments/assets/afa8753b-a0f2-4a61-9d51-b12c51979f35)
