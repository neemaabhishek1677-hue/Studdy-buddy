# Studdy-buddy
An AI-powered web app for first-year engineering students to get instant summaries, key points, flashcards, practice questions, and quizzes for any topic.

---

## 🚀 Features

- **AI-Generated Study Material** — Summary, Key Points, Flashcards, Practice Questions
- **Quiz Mode** — Multiple choice quiz with scoring
- **Save Notes** — Persist study notes locally via localStorage
- **Dashboard** — View all saved topics at a glance
- **Difficulty Levels** — Easy, Medium, Hard
- **Quick Topics** — One-click demo topics for instant generation

---

## 🛠️ Tech Stack

| Layer      | Technology                  |
|------------|-----------------------------|
| Frontend   | React (Create React App)    |
| Backend    | Node.js + Express           |
| AI         | Anthropic Claude API        |
| Styling    | Plain CSS with CSS Variables|
| Storage    | localStorage (client-side)  |

---

## 📁 Project Structure

```
studybuddy/
├── public/
│   └── index.html
├── src/
│   ├── components/
│   │   ├── Sidebar.js
│   │   └── Sidebar.css
│   ├── pages/
│   │   ├── Dashboard.js
│   │   ├── Dashboard.css
│   │   ├── StudyPage.js
│   │   └── StudyPage.css
│   ├── App.js
│   ├── App.css
│   ├── index.js
│   └── index.css
├── backend/
│   ├── server.js
│   ├── package.json
│   └── .env.example
├── package.json
├── .gitignore
└── README.md
```

---

## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/studybuddy.git
cd studybuddy
```

### 2. Setup the Backend

```bash
cd backend
npm install
cp .env.example .env
# Edit .env and add your Anthropic API key
```

Get your API key from: https://console.anthropic.com

```bash
npm run dev   # starts backend on http://localhost:5000
```

### 3. Setup the Frontend

In a new terminal, from the root of the project:

```bash
npm install
npm start     # starts frontend on http://localhost:3000
```

The frontend is pre-configured to proxy API requests to `localhost:5000` via the `"proxy"` field in `package.json`.

---

## 🔑 Environment Variables

Create `backend/.env`:

```env
ANTHROPIC_API_KEY=your_api_key_here
PORT=5000
```

---

## 📸 Demo Topics

The app comes with 6 pre-configured demo topics:
1. Newton's Laws of Motion (Physics)
2. Binary Search Trees (DSA)
3. Ohm's Law & Circuits (Electronics)
4. Thermodynamics Basics (Mechanical)
5. OSI Network Model (Networking)
6. Probability & Statistics (Maths)

---

## 🚢 Deployment

**Frontend** → Deploy to Vercel / Netlify  
**Backend** → Deploy to Render / Railway / Heroku

Make sure to set `ANTHROPIC_API_KEY` as an environment variable in your hosting platform.
