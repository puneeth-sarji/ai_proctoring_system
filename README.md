# ai_proctoring_system
# Risk-Based Proctoring System for Online Assessments

## Overview
This project introduces a privacy-friendly, risk-based proctoring system that ensures academic integrity without relying on intrusive video surveillance. The system leverages behavioral analysis, real-time risk scoring, and machine learning anomaly detection to detect potential cheating while maintaining user privacy.

## Problem Statement
The challenge is to create a secure online assessment environment without using webcam-based monitoring. Instead, the system should analyze non-invasive behavioral inputs such as:
- Mouse movements
- Keystroke patterns
- Activity shifts

## Solution
Our system provides:
- **Real-time risk scoring** based on user behavior
- **Hybrid detection approach** using rule-based and ML-based anomaly detection
- **Automated flagging system** for suspicious activities
- **Privacy-compliant monitoring** without webcam or microphone usage

## Key Features
- **Privacy-Compliant Monitoring**: No intrusive video or audio tracking.
- **Hybrid Detection Approach**: Combination of rule-based and machine learning techniques.
- **Real-Time Risk Scoring**: Instant assessment of behavioral anomalies.
- **Adaptive and Scalable**: Works across multiple platforms and assessment types.
- **Non-Intrusive Analysis**: Tracks mouse movements, keystroke dynamics, and window activity shifts.
- **Automated Alerts**: Flags potential risks based on threshold scoring.
- **Future Enhancements**: AI-driven adaptability, multi-factor authentication, and broader cross-platform support.

## Technologies Used
### Frontend (User Interface)
- **Frameworks**: React.js/Angular with JavaScript for an interactive UI
- **Data Capture**: Keystroke dynamics, mouse movements, tab/window switching
- **Real-Time Feedback**: Alerts users to detected anomalies
- **Communication**: WebSockets/REST APIs for backend interaction
- **Security**: Bcrypt.js / JWT authentication for user session security

### Backend (Processing & Detection)
- **Frameworks**: Django/Flask (Python) or Node.js (Express)
- **Detection Engine**: Combination of rule-based heuristics and ML anomaly detection
- **Machine Learning**: Isolation Forests, Autoencoders, LSTMs (TensorFlow/PyTorch)
- **Storage**: PostgreSQL/MongoDB for logs, Redis for real-time event caching
- **Deployment**: Docker & Kubernetes for scalable cloud hosting on AWS
- **Security & Compliance**: GDPR compliance, encrypted storage, RBAC for access control

## Workflow
1. **User Authentication & Exam Initiation**
2. **Behavioral Data Capture**
3. **Data Processing & Feature Extraction**
4. **Rule-Based Detection**
5. **ML-Based Anomaly Detection**
6. **Risk Scoring & Alert System**
7. **Integration & Reporting for Exam Administrators**

## Advantages
- **Enhanced Exam Integrity**: Prevents cheating via behavioral analysis instead of intrusive surveillance.
- **Privacy-First Approach**: Ensures user trust and compliance with data protection laws.
- **Extensibility**: Can be integrated into multiple LMS and examination platforms.
- **Real-Time Fraud Detection**: Provides instant risk alerts.
- **AI-Driven Adaptability**: ML models improve detection over time.
- **Reduced Administrative Load**: Automates tracking, reducing manual intervention.
- **Audit & Review Capabilities**: Stores flagged behaviors for later analysis.

## Setup & Installation
### Prerequisites
- Node.js
- MongoDB/PostgreSQL
- Python (if using Django/Flask)
- Docker (optional for deployment)

### Steps to Run Locally
1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/proctoring-system.git
   cd proctoring-system
   ```
2. Install dependencies:
   ```sh
   npm install  # for frontend
   cd backend && pip install -r requirements.txt  # for Python backend
   ```
3. Set up environment variables in `.env`:
   ```sh
   MONGO_URI=mongodb://127.0.0.1:27017/proctorai_db
   JWT_SECRET=your_jwt_secret_key
   ```
4. Start the backend server:
   ```sh
   npm start  # for Node.js
   python manage.py runserver  # for Django
   ```
5. Start the frontend:
   ```sh
   cd frontend && npm start
   ```
6. Access the system at `http://localhost:3000`

## Future Enhancements
- AI-powered adaptive proctoring
- Multi-factor authentication for added security
- Expanded ML model training for improved accuracy
- Integration with third-party LMS platforms

## License
This project is licensed under the MIT License. Feel free to contribute and improve the system!

