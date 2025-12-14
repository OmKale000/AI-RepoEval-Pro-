# AI RepoEval Pro 🚀  
**AI-Powered GitHub Repository Evaluation & Developer Profiling**

AI RepoEval Pro is a web-based tool that analyzes a GitHub repository URL and generates a **structured evaluation report**, including a **score**, **technical summary**, **recruiter perspective**, **mentor guidance**, **interview questions**, and a **personalized improvement roadmap**.

The platform is designed for **students, mentors, and recruiters** to better understand the maturity and readiness of a developer’s GitHub projects.

---

## ✨ Key Features

- 🔍 **Repository Evaluation**
  - Accepts any public GitHub repository URL
  - Infers project type and structure from repository metadata
  - Generates a detailed, structured evaluation report

- 📊 **AI Scoring System**
  - Score out of 100 with maturity level (Beginner / Intermediate / Advanced)
  - Project completion index
  - Code quality and best-practice insights

- 🧠 **Dual Perspective Analysis**
  - **Recruiter View**: Hire-readiness, professionalism, and real-world relevance
  - **Mentor View**: Technical growth guidance and next steps

- 🛠️ **Personalized Improvement Roadmap**
  - Actionable, step-by-step recommendations to improve repository quality

- 🎯 **AI Interview Preparation**
  - Skill-based interview questions generated from inferred technologies

- ✍️ **Documentation Refiner**
  - Rewrites README text, commit messages, or documentation in multiple styles using AI

- 🎧 **Text-to-Speech Mentor Feedback**
  - Converts mentor feedback into audio using Gemini TTS

---

## 🏗️ Project Architecture

```
AI-RepoEval-Pro/
├── index.html          # Frontend UI (Tailwind CSS + Vanilla JS)
├── backend/
│   ├── server.js       # Node.js proxy server (Gemini API calls)
│   ├── package.json
│   ├── package-lock.json
│   └── .env            # Gemini API key (not committed)
├── .gitignore
└── README.md
```

---

## ⚠️ Important Design Note

> This project **does NOT directly scan GitHub code**.

Due to environment and permission constraints:
- The AI performs a **hypothetical analysis**
- Insights are inferred from the repository name, URL semantics, and common industry patterns
- This is clearly disclosed inside the application

This design choice ensures:
- Privacy safety
- Fast responses
- Hackathon feasibility

---

## 🛠️ Tech Stack

### Frontend
- HTML5  
- Tailwind CSS  
- Vanilla JavaScript (SPA-style navigation)

### Backend
- Node.js  
- Express.js  
- Gemini API (Google Generative Language API)

### AI Models Used
- `gemini-1.5-flash` – Text analysis & generation  
- `gemini-2.5-flash-preview-tts` – Text-to-speech  

---

## 🚀 How to Run the Project Locally

### 1️⃣ Prerequisites
- Node.js (v18 or above)
- A valid **Google Gemini API key**

---

### 2️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/AI-RepoEval-Pro.git
cd AI-RepoEval-Pro
```

---

### 3️⃣ Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file inside `backend/`:

```env
GEMINI_API_KEY=your_api_key_here
```

Start the backend server:

```bash
node server.js
```

Backend runs on:

```
http://localhost:3000
```

---

### 4️⃣ Frontend Setup

Open `index.html`

Ensure frontend API calls point to the backend:

```js
fetch("http://localhost:3000/analyze", { ... })
```

Then open `index.html` in your browser (Chrome recommended).

---

## 🧪 How to Use the Application

1. Open the app in your browser  
2. Navigate to **Evaluator**  
3. Paste a public GitHub repository URL  

```
https://github.com/username/repository-name
```

4. Click **Analyze Repository**
5. Review:
   - Score & maturity level
   - Summary and evaluation
   - Improvement roadmap
   - Interview questions
6. (Optional) Use **Documentation Refiner** to polish text

---

## 🔐 Security & Privacy

- API keys are stored **only in `.env`**
- `.gitignore` prevents accidental key leaks
- No GitHub authentication or repository cloning is performed

---

## 🎓 Ideal Use Cases

- Students preparing portfolios
- Hackathon project evaluations
- Mentors reviewing student repositories
- Resume and GitHub profile improvement
- Interview preparation

---

## 👤 Author

**O.K.**  
Lead Engineer & Designer  

- GitHub: https://github.com/OmKale000  
- LinkedIn: https://www.linkedin.com/in/om-kale-1663a0276/  
- Email: ok176471@gmail.com  


