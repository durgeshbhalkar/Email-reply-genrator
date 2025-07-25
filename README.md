# 📧 AI-Powered Email Writer & Reply Generator

This is a full-stack web application that uses **Google Gemini AI** to generate professional, context-aware email replies. Built with **Spring Boot** for the backend and **React** for the frontend, it offers a seamless user experience for drafting human-like emails in multiple tones.

---

## 🚀 Features

- ✨ Generate professional and grammatically correct email content
- 🤖 Integrate with Google Gemini AI API (Generative Language)
- 🧠 Choose tone: formal, friendly, or professional
- 🔗 REST API built with Spring Boot
- 🖥️ Interactive frontend built with React
- ⚡ Fast response time (under 500ms)

---

## 🛠️ Tech Stack

| Layer     | Technology                  |
|-----------|-----------------------------|
| Backend   | Java, Spring Boot, Spring MVC |
| Frontend  | React, HTML, CSS, JavaScript |
| API       | Gemini Generative Language API |
| Build Tool| Maven                       |
| Testing   | Postman (API Testing)       |

---

## 📦 Project Structure

```bash
email-writer/
├── email-writer-sp/           # Spring Boot backend
│   ├── src/
│   ├── pom.xml
│   └── application.properties
├── email-writer-frontend/     # React frontend
│   ├── public/
│   ├── src/
│   └── package.json
└── README.md
```

Request Body
POST /api/email/generate
{
  "emailContent": "Hi, I saw your resume and wanted to follow up on the position..."
  "tone": "formal",
}

⚙️ Configuration
1. Set your Gemini API Key
In application.properties (Spring Boot)

gemini.api.url=https://generativelanguage.googleapis.com/v1beta/models/gemini-1.5-flash:generateContent
gemini.api.key=YOUR_GEMINI_API_KEY
server.port=8000

🔧 Run Locally
Backend
cd email-writer-sp
./mvnw spring-boot:run

Frontend
cd email-writer-frontend
npm install
npm start


✅ Future Enhancements
🌐 Language translation support

📁 Save email history per user

🛡️ Add authentication (JWT/Session)

🧾 Download generated emails as .txt or .pdf
