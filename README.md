# Apricity.ai

Apricity.ai is an intelligent, full-stack learning platform designed to help students study more effectively. By combining Retrieval-Augmented Generation (RAG), AI-generated quizzes, YouTube video recommendations, and productivity tracking, Apricity.ai turns study materials into interactive learning spaces.

**Live App:** [https://apricity-ai-seven.vercel.app](https://apricity-ai-seven.vercel.app)  
**Backend API:** [https://apricity-server.onrender.com](https://apricity-server.onrender.com)

---

## Features

- **Document Q&A (RAG):** Upload PDF study materials and ask questions with direct page citations.
- **AI-Powered Tutor (Gini):** Conversational AI tutor supporting voice input, concise/in-depth answer modes, and multi-modal vision analysis.
- **Dynamic Model Selector:** Switch between Google Gemini models (`gemini-2.0-flash`, `gemini-2.0-flash-lite`).
- **Interactive Quiz Generator:** Automatically create multiple-choice, short-answer, and long-answer assessments from documents or topics.
- **YouTube Learning Recommendations:** Contextual video suggestions generated from chat interactions to reinforce key topics.
- **Productivity & Study Tracker:** Set long-term academic goals, track daily commitments, utilize a Pomodoro timer/stopwatch, and manage study task blocks.
- **Authentication:** Email & password authentication with Google OAuth 2.0 integration and email verification.

---

## Tech Stack

- **Frontend:** React, Vite, React Router, Vanilla CSS
- **Backend:** Node.js, Express, Mongoose, Passport.js (JWT & Google OAuth 2.0)
- **Database:** MongoDB Atlas
- **AI Integration:** Google Generative AI (`@google/generative-ai` SDK)
- **Cloud Storage & Mail:** Cloudinary, Nodemailer

---

## Project Structure

```
apricity-ai/
├── client/          # React + Vite Frontend
│   └── src/         # UI components, pages, API hooks, state management
└── server/          # Node.js + Express Backend
    └── src/         # Controllers, routes, models, middleware, AI logic
```

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/codeewithaddy/apricity-ai.git
cd apricity-ai
```

### 2. Install dependencies

```bash
# Install server dependencies
cd server && npm install

# Install client dependencies
cd ../client && npm install
```

### 3. Environment Setup

Create a `.env` file in the `server` directory with your credentials:

```env
PORT=5000
NODE_ENV=production
FRONTEND_URL=https://apricity-ai-seven.vercel.app
BACKEND_URL=https://apricity-server.onrender.com
MONGO_URI=your-mongodb-atlas-uri
GEMINI_API_KEY=your-gemini-api-key
GEMINI_MODEL=gemini-2.0-flash
JWT_SECRET=your-jwt-secret
SESSION_SECRET=your-session-secret
CLOUDINARY_CLOUD_NAME=your-cloudinary-cloud-name
CLOUDINARY_API_KEY=your-cloudinary-api-key
CLOUDINARY_API_SECRET=your-cloudinary-api-secret
EMAIL_HOST=smtp.gmail.com
EMAIL_PORT=587
EMAIL_USER=your-email@gmail.com
EMAIL_PASS=your-app-password
GOOGLE_CLIENT_ID=your-google-client-id
GOOGLE_CLIENT_SECRET=your-google-client-secret
GOOGLE_CALLBACK_URL=https://apricity-server.onrender.com/api/auth/google/callback
```

### 4. Run the application

```bash
# Terminal 1 — Start Backend Server
cd server && npm run dev

# Terminal 2 — Start Frontend Client
cd client && npm run dev
```

---

## Deployment

- **Frontend:** Deployed on Vercel with single-page application routing.
- **Backend:** Deployed on Render Web Services connected to MongoDB Atlas.

---

## Author

Created by **Adarsh Gupta**  
- **GitHub:** [https://github.com/codeewithaddy/](https://github.com/codeewithaddy/)  
- **LinkedIn:** [https://www.linkedin.com/in/creationwithaddy/](https://www.linkedin.com/in/creationwithaddy/)
