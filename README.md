# AI-Powered Patient Risk Prediction System

**June 2024**

## Overview
The AI-Powered Patient Risk Prediction System is a full-stack application designed to assist healthcare providers in identifying high-risk patients for conditions such as diabetes and hypertension. By leveraging machine learning models trained on historical data, this system aims to help providers proactively manage patient health.

## Features
- **Real-Time Patient Monitoring:** Frontend dashboard for viewing real-time patient risk levels.
- **Risk Prediction Models:** Uses machine learning models to predict risks for specific health conditions.
- **Secure Data Management:** Stores patient data securely with SQL, ensuring quick access and scalable storage.
- **Continuous Integration & Deployment:** Automated CI/CD with Jenkins for smooth and reliable updates.

## Tech Stack
- **Frontend:** React, TypeScript
- **Backend:** Java Spring Boot
- **Machine Learning Models:** Python (TensorFlow/PyTorch)
- **Database:** SQL
- **CI/CD:** Jenkins

## Installation

### Prerequisites
1. Node.js (for React frontend)
2. Java (for Spring Boot backend)
3. Python (for training ML models)
4. SQL-compatible database (e.g., MySQL, PostgreSQL)
5. Jenkins (for CI/CD setup)

### Steps
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/your-repo-url
   cd patient-risk-prediction
   ```

2. **Frontend Setup:**
   ```bash
   cd frontend
   npm install
   npm start
   ```

3. **Backend Setup:**
   ```bash
   cd ../backend
   ./mvnw spring-boot:run
   ```

4. **Database Setup:**
   - Configure your SQL database and update connection strings in the backend `application.properties`.

5. **CI/CD Setup (Jenkins):**
   - Set up Jenkins jobs to automate deployment for both the frontend and backend.

## Usage
1. **Access the Dashboard:** Open the frontend in a browser to view patient risk statuses and predictions.
2. **Data Input:** Load patient data (historical and real-time) into the database for accurate model predictions.
3. **Monitor & Manage:** Use the dashboard to monitor and manage high-risk patients effectively.

## Contributing
1. Fork the repository.
2. Create a new branch.
3. Make your changes and submit a pull request.

