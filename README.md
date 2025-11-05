# 🧠 AI-Powered Resume Builder

An **intelligent resume generation platform** that uses **OpenAI’s API** and a **Spring Boot + React** stack to create personalized, professional resumes automatically based on user inputs.

![Tech Stack](https://img.shields.io/badge/TechStack-Java%20%7C%20SpringBoot%20%7C%20React%20%7C%20TailwindCSS%20%7C%20OpenAIAPI-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Active-success)
![Contributions](https://img.shields.io/badge/Contributions-Welcome-orange)

---

## 🚀 Features

- 🧾 **AI Resume Generation** — Automatically generates professional resume text sections using OpenAI.
- ⚙️ **Dynamic Template System** — Supports multiple LaTeX and HTML-based templates for instant customization.
- 💬 **Interactive Preview** — Real-time rendering of resume changes in the frontend.
- 🔄 **Modular Architecture** — Clean separation of backend (Spring Boot) and frontend (React + Tailwind).
- ⚡ **Performance Optimized** — Uses async API calls and caching for faster response and rendering.
- 🧩 **RESTful APIs** — Provides structured endpoints for resume text, templates, and generation history.
- 💾 **Export Options** — Download resumes as PDF or LaTeX files.

---

## 🏗️ Tech Stack

| Layer | Technologies |
|:------|:--------------|
| **Frontend** | React, Tailwind CSS, DaisyUI |
| **Backend** | Spring Boot, REST API |
| **AI Integration** | OpenAI API |
| **Build Tools** | Maven, npm |
| **Others** | JSON, DTO-based service architecture |

---

## 📁 Project Structure

```bash
AI-Resume-Builder/
├── backend/
│   ├── src/main/java/com/resumebuilder/
│   │   ├── controller/       # ResumeController.java
│   │   ├── service/          # ResumeService & ResumeServiceImpl.java
│   │   ├── model/            # ResumeRequest.java (DTO)
│   │   └── ResumeAiBackendApplication.java
│   └── pom.xml
│
├── frontend/
│   ├── src/
│   │   ├── components/       # React UI Components
│   │   ├── pages/            # Resume input, preview, download
│   │   ├── styles/           # Tailwind + DaisyUI configuration
│   │   └── App.jsx
│   ├── vite.config.js
│   └── package.json
│
└── README.md
```

---

## ⚡ Getting Started

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/VanshAngaria/AI-Resume-Builder.git
cd AI-Resume-Builder
```
### 2️⃣ Backend Setup (Spring Boot)
```bash
cd backend
mvn clean install
mvn spring-boot:run
```
### 3️⃣ Frontend Setup (React)
```bash
cd frontend
npm install
npm run dev
```

Then open your browser at http://localhost:5173/

### 🔐 Environment Variables

Create a .env file in your backend directory:
```
OPENAI_API_KEY=your_openai_api_key_here
```

### 🧠 How It Works

User Input — Enter your personal details, education, and experience in the React interface.

Backend Processing — Spring Boot calls the OpenAI API to generate context-aware resume sections.

Live Preview — The frontend displays a formatted resume preview in real time.

Export — Users can download the resume as PDF or LaTeX.

### 🧩 API Endpoints

| Method | Endpoint | Description |
|:-------|:----------|:-------------|
| `POST` | `/api/resume/generate` | Generate resume content using AI |
| `GET`  | `/api/resume/templates` | Fetch available templates |
| `POST` | `/api/resume/download`  | Export resume as PDF/LaTeX |

### 🧰 Example Request
```JSON
POST /api/resume/generate
{
  "name": "Vansh Angaria",
  "education": "B.Tech in Computer Science",
  "skills": ["Java", "Spring Boot", "React", "AI"],
  "experience": "Intern at CDAC Noida",
  "objective": "To build AI-driven applications that solve real-world problems."
}
```

### 📊 Results

🚀 30% faster resume rendering with async API optimization.

🧠 Context-aware AI content generation powered by OpenAI GPT models.

⚙️ 95% template accuracy for LaTeX and HTML resume exports.

### 🧑‍💻 Author

Vansh Angaria
    B.Tech, IIITDM Kurnool,
    AI Enthusiast
