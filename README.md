# Apricity.ai ☀️

> An AI-powered full-stack learning companion app featuring RAG-driven document Q&A, interactive quizzes, YouTube learning recommendations, and study goal management.

---

## ✨ Features

- 📄 **RAG Document Q&A**: Upload PDFs and ask questions with precise page citations.
- ⚡ **Free Gemini Model Selector**: Switch dynamically between free tier models (`gemini-2.0-flash`, `gemini-2.0-flash-lite`, `gemini-2.5-flash`, `gemini-1.5-flash`).
- 📝 **AI Quiz Generator**: Generate MCQs, short answers, and long answers from your study documents or custom topics.
- 📺 **YouTube Recommendations**: Get contextual YouTube video suggestions based on chat discussions.
- 🎯 **Study Companion**: Set long-term goals, track daily commitments, utilize the Pomodoro timer/stopwatch, and manage to-do lists.
- 🔐 **Secure Authentication**: Email & password authentication with Google OAuth 2.0 integration.

---

## 🛠️ Tech Stack

- **Frontend**: React, Vite, React Router, Vanilla CSS (Warm Slate & Amber Theme).
- **Backend**: Node.js, Express, Mongoose, Passport.js (JWT & Google OAuth).
- **Database**: MongoDB Atlas.
- **AI Engine**: Google Generative AI (`@google/generative-ai` SDK).
- **Storage & Mail**: Cloudinary, Nodemailer.

---

## 🚀 Quick Start

### 1. Clone the repository
```bash
git clone https://github.com/codeewithaddy/apricity-ai.git
cd apricity-ai
```

### 2. Install dependencies
```bash
# Install root dependencies
npm install

# Install server dependencies
cd server && npm install

# Install client dependencies
cd ../client && npm install
```

### 3. Configure Environment Variables
Create `.env` inside `server/`:
```env
NODE_ENV=development
FRONTEND_URL=http://localhost:5173
BACKEND_URL=http://localhost:5000
GEMINI_API_KEY=your-gemini-api-key
GEMINI_MODEL=gemini-2.0-flash
MONGO_URI=your-mongodb-atlas-uri
JWT_SECRET=your-jwt-secret
SESSION_SECRET=your-session-secret
```

### 4. Run Locally
```bash
# Terminal 1 — Backend
cd server && npm run dev

# Terminal 2 — Frontend
cd client && npm run dev
```

Open `http://localhost:5173/` in your browser.
