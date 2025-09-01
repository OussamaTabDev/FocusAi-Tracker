# 🌟 FocusAI Tracker

A comprehensive Windows desktop application that helps users understand and improve their computer usage habits through AI-powered insights, productivity tracking, and intelligent parental controls.

---

## 🎯 Overview

FocusAI Tracker combines the power of AI with comprehensive activity monitoring to provide users with actionable insights about their computer usage. Whether you're a professional looking to boost productivity or a parent wanting to ensure safe computer use for your children, FocusAI Tracker has you covered.

Built with a **Python backend** and a **React + Auri desktop frontend**, the app offers the performance of native apps without the bloat of Electron.

---

## 🏗️ Architecture

FocusAI Tracker uses a hybrid architecture with a **Python Flask backend** and a **React/Auri frontend**. Auri serves as the lightweight desktop runtime, providing native system integration (tray menus, notifications, file system access) while keeping resource usage minimal compared to Electron.

### Technology Stack

**Frontend:**

* **Auri**: Cross-platform desktop application shell (native integration, low overhead)
* **React (TypeScript)**: Modern UI framework
* **Tailwind CSS**: Utility-first CSS framework
* **Chart.js** + **react-chartjs-2**: Rich data visualization
* **Lucide-react**, **date-fns**, **axios**, **@headlessui/react**

**Backend:**

* **Python 3.9+**, **Flask**, **Flask-SQLAlchemy**, **SQLite**
* **Cryptography**, **psutil**, **pywin32**, **pillow**, **schedule**

---

## 💻 Development Setup

### Development Servers

```bash
# Terminal 1: Start Python backend
cd backend
python run.py

# Terminal 2: Start React frontend (web dev mode)
cd frontend
npm start

# Terminal 3: Package & run desktop with Auri
cd frontend
npm run auri-dev
```

👉 Unlike Electron, Auri doesn’t bundle Chromium — it uses the system webview, meaning **faster startup, less memory usage, and smaller builds**.

---

## 🚀 Installation

End users will install a **native Auri-powered app** packaged as a Windows installer (`FocusAI-Tracker-Setup.exe`). No Node.js runtime or heavy dependencies are required at runtime.

---

## 🙏 Acknowledgments

* **Google Gemini**: AI-powered insights and recommendations (planned)
* **Auri Framework**: Lightweight cross-platform desktop runtime powering the app shell
* **Python Community**: Backend ecosystem
* **Contributors**: All developers who help improve FocusAI Tracker


