# TeamPulse - Frontend Client

Frontend client for **TeamPulse**, built entirely with pure **Vanilla JavaScript, HTML5, and CSS3** (no external framework dependencies). Communicates with the Spring Boot backend via REST APIs and WebSockets.

---

## 📂 Repository Structure
```
.
├── README.md
├── .gitignore
└── frontend/
    ├── index.html        # Landing page & navigation
    ├── login.html        # User login (supports username or email)
    ├── register.html     # User registration form
    ├── dashboard.html    # User workspaces & analytics dashboard
    └── workspace.html    # Real-time channels, messaging, and sentiment analysis
```

---

## 🛠️ Features
- **Pure Vanilla JS:** Lightweight, zero bundle overhead, runs natively in any modern browser.
- **Responsive Modern UI:** Dark mode styling with fluid layouts and animations.
- **REST & Real-Time:** Integrates with the TeamPulse Spring Boot backend on port `3333`.
- **Pages:**
  - `login.html`: Authenticates users with username or email.
  - `register.html`: Validates inputs and creates new accounts.
  - `dashboard.html`: Displays team workspaces, stats, and rankings.
  - `workspace.html`: Real-time chat channels, messages, and sentiment analysis.

---

## 🚀 Running Locally

To avoid CORS and browser file-origin restrictions, serve the `frontend` folder using any local HTTP static server:

### Option 1: Python HTTP Server (Recommended)
```bash
cd frontend
python -m http.server 5500
```
Open [http://localhost:5500/login.html](http://localhost:5500/login.html) in your browser.

### Option 2: VS Code Live Server
1. Open the `frontend` folder in VS Code.
2. Click **Go Live** on the bottom status bar.

### Option 3: Node.js `serve` / `http-server`
```bash
npx serve frontend -p 5500
```

---

## ⚙️ Backend Connection - Open [Backend Repo Link](https://github.com/tejrohitparuchuri/tt-3-1-backend-ext)
The frontend expects the Spring Boot backend running at `http://localhost:3333`. Ensure CORS is enabled on the backend server.
