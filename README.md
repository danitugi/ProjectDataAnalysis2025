
# 🏙️ Tel Aviv Apartment Rent Predictor 🧠  
*Final Project – Data Analyst Course 2025 | Full Project*

[![Python](https://img.shields.io/badge/Python-3.9+-blue?logo=python)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Processing-lightgrey?logo=pandas)]
[![Scikit-learn](https://img.shields.io/badge/ML-scikit--learn-orange?logo=scikit-learn)]
[![Flask](https://img.shields.io/badge/API-Flask-000?logo=flask)]
[![BeautifulSoup](https://img.shields.io/badge/Web%20Scraping-BeautifulSoup4-green?logo=html5)]
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 🧾 Project Overview

This is the final project for the **Data Analyst Course – 2025**, focused on predicting **apartment rental prices in Tel Aviv** using real-world data.

The project is divided into 3 parts:

- **Part A**: Data collection via web scraping  - https://github.com/danitugi/ProjectDataAnalysis2025_PartA
- **Part B**: Data preprocessing & Machine Learning modeling  - https://github.com/danitugi/ProjectDataAnalysis2025
- **Part C**: Deployment of a web app using Flask  - https://github.com/danitugi/ProjectDataAnalysis2025_PartC

---

## 🔍 Part A – Data Collection

We scraped listings from [ad.co.il](https://www.ad.co.il/nadlanrent) for Tel Aviv rental apartments using `BeautifulSoup` and stored the data in a structured `.csv` file.

- Included Features: apartment details, location, amenities, and prices  
- Additional Feature: calculated distance from Tel Aviv city center via geolocation

📄 Output: `train.csv`

---

## 🤖 Part B – Modeling

We cleaned and transformed the dataset to fit a strict schema and trained two regression models:

- **Elastic Net Regression**
- **Tree-Based Regressor** (e.g., Random Forest or Gradient Boosting)

We compared model performance using **Mean Squared Error (MSE)** and selected the best model for deployment.

📄 Output: `trained_model.pkl` (or `.joblib`)

---

## 🌐 Part C – Web Application

We developed a full web app using **Flask** and HTML/CSS UI, allowing users to:

- Input apartment details via form
- Submit data and get a predicted rental price in real-time
- View a stylish interface with RTL Hebrew support and animations

📁 Main files:
- `api.py` – Flask backend  
- `templates/index.html` – HTML UI  
- `model_training.py` – model training and export script

---

## 📁 Project Structure

```
├── flask_rent_app/
│   ├── api.py
│   ├── model_training.py
│   ├── trained_model.joblib
│   ├── train.csv
│   ├── templates/
│   │   └── index.html
│   └── static/ (optional)
├── README.md
└── requirements.txt
```

---

## 🚀 How to Run Locally

1. Clone the repo:
```bash
git clone https://github.com/yourusername/tel-aviv-rent-predictor.git
cd tel-aviv-rent-predictor/flask_rent_app
```

2. Create virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install requirements:
```bash
pip install -r requirements.txt
```

4. Train model (if needed):
```bash
python model_training.py
```

5. Run app:
```bash
python api.py
```

6. Open in browser:
```
http://127.0.0.1:5000/
```

---

## 🧠 Technologies Used

- Python 3.9+
- pandas, numpy, scikit-learn, joblib
- BeautifulSoup (Web Scraping)
- Flask (Web App & API)
- HTML + CSS (Frontend)

---

## 📄 License

This project is licensed under the **MIT License**.

---

## 🙌 Authors

*Daniel T. – Data Analyst Final Project @ 2025 Cohort*
