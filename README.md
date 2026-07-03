# GramKavach
Cybersecurity alert system
# 🛡️ Gram-Kavach: AI-Powered Rural Fraud Protection

<div align="center">
  <img src="https://img.shields.io/badge/Status-Hackathon_Project-FF9900?style=for-the-badge" alt="Status"/>
  <img src="https://img.shields.io/badge/Frontend-React-20232a?style=for-the-badge&logo=react" alt="React"/>
  <img src="https://img.shields.io/badge/Backend-FastAPI-009688?style=for-the-badge&logo=fastapi" alt="FastAPI"/>
  <img src="https://img.shields.io/badge/AI-Bhashini_API-blue?style=for-the-badge" alt="Bhashini"/>
</div>

## 📌 Project Overview
**Gram-Kavach** is a multilingual, AI-driven fraud detection platform designed to protect rural populations from digital and telephonic scams. Built during a fast-paced hackathon, this solution bridges the digital divide by analyzing suspicious messages and calls in regional languages and providing real-time alerts to vulnerable users.

### 🎯 The Problem
Rural and non-English speaking demographics are increasingly targeted by sophisticated phishing and financial scams. Existing fraud detection tools predominantly cater to English speakers, leaving a massive population unprotected.

### 💡 The Solution
Gram-Kavach leverages artificial intelligence to analyze communication patterns and flag fraudulent intent. By integrating with the Bhashini API, it processes regional languages seamlessly, and utilizes Twilio to immediately dispatch SMS alerts to users or their registered family members when a threat is detected.

---

## 🛠️ Tech Stack & Integrations

*   **Frontend:** React.js (Tailwind CSS for responsive UI)
*   **Backend:** Python, FastAPI
*   **AI/NLP:** Bhashini API (Multilingual Translation & Processing)
*   **Alerting/Communication:** Twilio API (SMS Notifications)
*   **Security:** JWT Authentication, Input Sanitization

---

## 🚀 Key Features

*   **Multilingual Threat Analysis:** Translates and analyzes regional language texts and audio transcripts for scam indicators.
*   **Real-Time SMS Alerts:** Instantly notifies users (and optionally, trusted contacts) of high-risk interactions via Twilio.
*   **Accessible Dashboard:** A highly intuitive React-based user interface tailored for ease of use by non-technical individuals.
*   **Lightweight & Fast:** Powered by FastAPI to ensure low-latency processing of incoming data streams.

---

## ⚙️ Local Setup & Installation

```bash
# 1. Clone the repository
git clone [https://github.com/Pratikshaprabhakarbande/GramKavach.git](https://github.com/Pratikshaprabhakarbande/GramKavach.git)

# 2. Navigate to the backend directory and install dependencies
cd GramKavach/backend
pip install -r requirements.txt

# 3. Configure API Keys
# Create a .env file in the backend folder and add your Twilio and Bhashini API credentials
# TWILIO_ACCOUNT_SID=your_sid
# TWILIO_AUTH_TOKEN=your_token
# BHASHINI_API_KEY=your_api_key

# 4. Start the FastAPI server
uvicorn main:app --reload

# 5. Open a new terminal, navigate to the frontend, and start the React app
cd ../frontend
npm install
npm start
