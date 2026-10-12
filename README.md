## ``Try my project here : ``[TeamPulse](teampulsebyptr.web.app)

# TeamPulse - Frontend Client

Frontend client for **TeamPulse**, built entirely with pure **Vanilla JavaScript, HTML5, and CSS3** (zero runtime framework overhead). Communicates directly with the Spring Boot backend via REST APIs.

---

## 🔗 Related Repositories

- **Main Full-Stack Repository:** [tejrohitparuchuri/TeamPulse](https://github.com/tejrohitparuchuri/TeamPulse)
- **Backend Service Repository:** [tejrohitparuchuri/tt-3-1-backend-ext](https://github.com/tejrohitparuchuri/tt-3-1-backend-ext)

---

## 📂 Repository Structure
```
.
├── README.md
├── .gitignore
└── frontend/
    ├── index.html        # Landing page & navigation
    ├── login.html        # User login (supports username or email)
    ├── register.html     # User registration with live username check
    ├── dashboard.html    # User workspaces & management dashboard
    └── workspace.html    # Channels, messaging, and live engagement rankings
```

---

## 🛠️ Features
- **Pure Vanilla JS:** Lightweight, zero bundle overhead, runs natively in any modern browser.
- **Responsive Dark Mode UI:** Modern sleek styling with micro-animations and intuitive navigation.
- **Direct REST Integration:** Directly connects to the TeamPulse Spring Boot backend on port `3333`.
- **Pages:**
  - `index.html`: Product overview and landing page.
  - `login.html`: Authenticates users with username or email.
  - `register.html`: Real-time username verification and account registration.
  - `dashboard.html`: Workspaces list, join workspace via code, and create new workspace.
  - `workspace.html`: Real-time messaging, unsent draft auto-saving, channels, and member leaderboard.

---

## 🚀 Running Locally

Serve the `frontend/` directory using any local static HTTP server:

### Option 1: Python HTTP Server (Recommended)
```bash
cd frontend
python -m http.server 5500
```
Open [http://localhost:5500/login.html](http://localhost:5500/login.html) in your browser.

### Option 2: VS Code Live Server
1. Open the `frontend/` folder in VS Code.
2. Click **Go Live** on the bottom status bar.

### Option 3: Node.js `serve` / `http-server`
```bash
npx serve frontend -p 5500
```

---

## ⚙️ Backend Connection
The frontend communicates directly with the Spring Boot backend running at `http://localhost:3333`. Ensure the backend server is running and MySQL is active.
