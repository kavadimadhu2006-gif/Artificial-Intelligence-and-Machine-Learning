gg# 🌊 Flood Prediction System using Machine Learning

## Project Overview

Floods are among the most destructive natural disasters, causing significant loss of life, damage to infrastructure, and economic disruption every year. Traditional flood forecasting methods often fail to provide timely and accurate warnings, limiting the ability of authorities to take preventive action.

This project presents a **Machine Learning-based Flood Prediction System** that predicts the likelihood of flood events using historical weather and environmental data. Multiple supervised learning algorithms including **Decision Tree**, **Random Forest**, **K-Nearest Neighbors (KNN)**, and **XGBoost** are trained and evaluated to identify the most accurate prediction model.

The best-performing model (**XGBoost**) is integrated into a **Flask Web Application**, allowing users to enter weather parameters and instantly receive flood risk predictions through a simple web interface. The application is designed to support future deployment on **IBM Cloud** for remote accessibility and scalability.

---

# Features

- Predict flood occurrence using Machine Learning
- User-friendly Flask web interface
- Multiple ML algorithms comparison
- Real-time prediction
- Model performance visualization
- Historical dataset training
- High prediction accuracy (96.55%)
- Ready for IBM Cloud deployment

---

# Machine Learning Algorithms Used

- Decision Tree
- Random Forest
- K-Nearest Neighbors (KNN)
- XGBoost (Best Model)

---

# Technologies Used

### Programming Language
- Python 3.8+

### Libraries
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-Learn
- XGBoost
- Joblib

### Web Framework
- Flask

### Frontend
- HTML
- CSS
- JavaScript

### Development Tools
- Jupyter Notebook
- VS Code
- Anaconda Navigator

### Deployment
- IBM Cloud (Optional)

---

# System Architecture

```
Weather Dataset
       │
       ▼
Data Preprocessing
       │
       ▼
Feature Selection
       │
       ▼
Model Training
       │
       ▼
Model Evaluation
       │
       ▼
Best Model (XGBoost)
       │
       ▼
Model Saved (.pkl)
       │
       ▼
Flask Web Application
       │
       ▼
Flood Prediction Result
```

---

# Dataset Features

The model is trained using the following weather parameters:

- Annual Rainfall (mm)
- Seasonal Rainfall (mm)
- Cloud Visibility (km)
- Humidity (%)
- Temperature (°C)
- River Water Level (m)
- Wind Speed (km/h)
- Pressure (hPa)
- Cloud Cover (%)
- Rainfall Intensity (mm/h)
- Month
- District

Target Variable:

- Flood (Yes / No)

---

# Project Structure

```
Flood-Prediction-System/

│
├── dataset/
│     flood_dataset.csv
│
├── model/
│     flood_model.pkl
│
├── static/
│     css/
│     images/
│
├── templates/
│     index.html
│     result.html
│
├── app.py
├── train_model.py
├── prediction.py
├── requirements.txt
├── README.md
└── LICENSE
```

---

# Installation

## Step 1

Clone the repository

```bash
git clone https://github.com/yourusername/Flood-Prediction-System.git
```

---

## Step 2

Go inside project

```bash
cd Flood-Prediction-System
```

---

## Step 3

Create Virtual Environment

Windows

```bash
python -m venv venv
```

Activate

```bash
venv\Scripts\activate
```

Linux/macOS

```bash
source venv/bin/activate
```

---

## Step 4

Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Step 5

Train Model

```bash
python train_model.py
```

This generates

```
flood_model.pkl
```

---

## Step 6

Run Flask Application

```bash
python app.py
```

---

## Step 7

Open Browser

```
http://127.0.0.1:5000/
```

---

# Project Workflow

1. Load historical weather dataset.
2. Clean missing values.
3. Encode categorical data.
4. Normalize numerical features.
5. Split training and testing datasets.
6. Train multiple ML models.
7. Compare model performance.
8. Save the best-performing model.
9. Integrate model into Flask.
10. Predict flood risk from user input.

---

# Model Performance

| Algorithm | Accuracy |
|------------|-----------|
| Decision Tree | 91.84% |
| Random Forest | 94.67% |
| KNN | 92.48% |
| **XGBoost** | **96.55%** |

Best Model:
**XGBoost**

---

# Project Scenarios

## Scenario 1: Early Flood Warning

A meteorologist enters current rainfall, humidity, and cloud visibility for a flood-prone district. The model predicts a high probability of flooding, enabling authorities to issue evacuation alerts before the disaster occurs.

---

## Scenario 2: Disaster Response

During monsoon season, disaster management officials monitor multiple regions simultaneously. The application provides instant flood risk predictions, helping prioritize rescue teams and emergency resources.

---

## Scenario 3: Model Validation

Government analysts validate the trained model using historical flood records. The XGBoost model achieves **96.55% accuracy**, demonstrating reliable performance for operational deployment.

---

# Hardware Requirements

- Intel Core i3 Processor or above
- Minimum 4 GB RAM
- 2 GB Free Storage
- Internet Connection

---

# Software Requirements

- Windows / Linux / macOS
- Python 3.8+
- Anaconda Navigator
- Jupyter Notebook
- Flask
- HTML
- CSS
- JavaScript
- IBM Cloud Account (Optional)

---

# Future Enhancements

- Live weather API integration
- SMS and Email flood alerts
- Mobile application
- GIS map visualization
- Real-time river sensor integration
- Satellite image analysis
- Deep Learning prediction models
- Multi-language support
- Cloud deployment on IBM Cloud
- IoT-based flood monitoring

---

# Skills Used

- Machine Learning
- Supervised Learning
- Decision Tree
- Random Forest
- K-Nearest Neighbors
- XGBoost
- NumPy
- Pandas
- Matplotlib
- Scikit-Learn
- Flask
- HTML
- CSS
- JavaScript
- Python

---

# Team Members

| Name | Role |
|------|------|
| Govula Jaya Prakash Reddy | Team Lead |
| Yerukala Madhu | Member |
| V. Yuva Kishore | Member |
| Peddisetty Usharani | Member |
| Y. R. Kiran Kumar | Member |

---

# Mentor

No mentor assigned.

---

# License

This project is developed for educational and research purposes.

---

# Acknowledgements

- IBM SkillsBuild
- Scikit-Learn
- XGBoost
- Flask
- Python Community
- Open Source Contributors

---

## Conclusion

The Flood Prediction System demonstrates how Machine Learning can improve disaster preparedness by accurately predicting flood events using weather and environmental data. By combining robust classification algorithms with a Flask-based web application, the system provides a practical, scalable, and user-friendly solution for early flood warning, disaster response, and decision-making. With an accuracy of **96.55%** achieved by the XGBoost model, the project offers a reliable foundation for future enhancements such as real-time weather integration, IoT sensor support, GIS mapping, and cloud deployment on IBM Cloud.
