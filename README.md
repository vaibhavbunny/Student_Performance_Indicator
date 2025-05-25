# 📊 Student Performance Predictor with MLOps Deployment

This project predicts student academic performance using socio-economic and educational attributes. It integrates Machine Learning modeling, interactive UI development with Flask, and MLOps deployment on AWS with CI/CD automation using GitHub Actions and Docker.

---

## 🚀 Features

* **Predictive Modeling**: Achieves \~90% R² score using regression models on student test data.
* **Data Analysis**: In-depth data cleaning, preprocessing, and EDA using Pandas, Matplotlib, and Seaborn.
* **ML Models Used**:

  * Linear Regression, Ridge, Lasso
  * Random Forest, SVM, KNN, Decision Tree
  * XGBoost, CatBoost, AdaBoost
* **Best Performing Models**:

  * Ridge Regression: 0.8805
  * Linear Regression: 0.8803
  * CatBoost Regressor: 0.8516

---

## 🧠 Tech Stack

| Component        | Technology                      |
| ---------------- | ------------------------------- |
| Language         | Python                          |
| ML Libraries     | Scikit-learn, XGBoost, CatBoost |
| Web Framework    | Flask                           |
| Visualization    | Matplotlib, Seaborn             |
| Containerization | Docker                          |
| Cloud            | AWS EC2, AWS ECR                |
| CI/CD            | GitHub Actions                  |
| UI               | HTML Templates, Streamlit       |

---

## 📂 Project Structure

```
├── app.py                  # Flask entry point
├── Dockerfile              # Docker setup
├── notebooks/              # EDA & model training
├── templates/              # HTML files
├── src/
│   ├── pipeline/           # Custom prediction pipeline
│   ├── components/         # Data ingestion, transformation, training
├── artifacts/              # Stored models and scalers
├── .github/workflows/      # CI/CD workflow definitions
├── requirements.txt        # Dependencies
└── setup.py                # Project packaging
```

---

## 🧪 How to Run Locally

```bash
# 1. Clone the repository
git clone https://github.com/vaibhavbunny/mlproject-aws-CI-CD-Projects.git
cd mlproject-aws-CI-CD-Projects

# 2. Create a virtual environment & activate
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Run Flask app
python app.py
```

Visit `http://localhost:5000` to use the web app.

---

## 🐳 Run with Docker

```bash
docker build -t student-performance-app .
docker run -p 5000:5000 student-performance-app
```

---

## ☁️ Deployment

* Deployed on **AWS EC2** with Docker
* Model artifacts stored on **AWS ECR**
* **GitHub Actions** automate training, testing, and deployment

---

## 📈 Results

| Model                   | R² Score |
| ----------------------- | -------- |
| Ridge Regression        | 0.8805   |
| Linear Regression       | 0.8803   |
| CatBoost Regressor      | 0.8516   |
| AdaBoost Regressor      | 0.8498   |
| Random Forest Regressor | 0.8472   |
| Lasso                   | 0.8253   |
| XGBRegressor            | 0.8216   |
| K-Neighbors Regressor   | 0.7838   |
| Decision Tree           | 0.7603   |



