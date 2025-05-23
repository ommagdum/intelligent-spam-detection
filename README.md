# ✉️ ML-Based Spam Email Detection Web App

🌐 **Live Demo**: [https://webapp-frontend-qawu.onrender.com/](https://webapp-frontend-qawu.onrender.com/)

> ⚠️ **Note:** Due to the limitations of Render’s free-tier hosting and traffic scaling constraints, initial loading of different modules (frontend, backend, and ML service) may take up to 30–60 seconds. Please allow some time for all services to wake up.

---

<div align="center">
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" />
  <img src="https://img.shields.io/badge/Spring_Boot-6DB33F?style=for-the-badge&logo=spring&logoColor=white" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" />
  <img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=JSON%20web%20tokens&logoColor=white" />
</div>

---

## 🧠 Project Overview

This web application detects spam emails in real time using a machine learning model hosted as a microservice. It offers:

- ✨ Real-time spam classification with confidence scores
- 🔐 Secure user login via JWT and Google OAuth2
- 📊 User dashboards and admin analytics
- 🔄 Feedback-based model retraining
- 📈 Historical analysis and prediction logs

---

## 🧩 Architecture

The application is split into 3 modules:

1. **Frontend**: Built with React + Tailwind CSS + Vite  
2. **Backend**: Spring Boot REST API with PostgreSQL and JWT-based auth  
3. **ML Service**: Python Flask app hosting a trained spam detection model

---

## 🚀 Tech Stack

### Frontend
- React 18 + Vite
- Tailwind CSS
- React Router v6
- JWT & Google OAuth2
- Chart.js, Axios, React Hook Form

### Backend
- Spring Boot 3.x
- PostgreSQL
- Spring Security, JWT, OAuth2
- Jakarta Validation, JavaMailSender
- Docker & Maven

### ML Model
- Python, Flask
- Scikit-learn, NLTK, TF-IDF
- Linear SVM with versioning and rollback
- Background training, metrics tracking

---

## ✨ Key Features

### 🔒 Authentication & Authorization
- JWT access/refresh token system
- Google OAuth2 sign-in
- Email verification for new users
- Role-based access control (User/Admin)

### 📧 Spam Detection
- ML-powered spam/ham classification
- Confidence scoring
- Feedback loop for continuous model improvement
- Model version rollback if performance drops

### 📊 Dashboard & Admin Tools
- Real-time analytics and user stats
- Full user management (admin panel)
- Trigger retraining and manage model versions
- Visualize prediction history

covert to markdown : convert to markdown : 
 📁 Repo Structure

```bash
/webapp-frontend # React app
/webapp-backend # Spring Boot API
/webapp-ml # Flask-based ML model API
```

🏃 Getting Started
1. Clone the Monorepo
```bash
git clone https://github.com/ommagdum/intelligent-spam-detection.git cd spam-detection-webapp
```

3. Setup Each Module
See individual module README files in `/frontend`, `/backend`, and `/ml-service` for installation and setup instructions.


📦 API Overview
Auth
* `POST /api/auth/register` – Register new user
* `POST /api/auth/login` – Login with credentials
* `GET /api/auth/verify` – Email verification
* `POST /api/auth/google-auth` – Google OAuth2
Spam Detection
* `POST /api/predict` – Run spam detection
* `GET /api/predictions/history` – Prediction logs
* `POST /api/feedback` – Feedback on prediction
Admin
* `GET /api/admin/users` – List all users
* `POST /api/admin/retraining/trigger` – Retrain ML model
* `GET /api/admin/stats` – System analytics
🧪 Testing
* Frontend: `npm test`
* Backend: `mvn test`
* ML service: `pytest` (optional)

🤝 Contributing
We welcome contributions!
1. Fork this repo
2. Create a branch (`git checkout -b feature/my-feature`)
3. Commit and push (`git commit -m "Add my feature"`)
4. Open a Pull Request 🎉

📄 License
This project is licensed under the **MIT License**.

📬 Contact
Have questions? Open an issue or reach out via GitHub.
