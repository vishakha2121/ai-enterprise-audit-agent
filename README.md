# 🚀 AI Enterprise Audit Agent

![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python)
![FastAPI](https://img.shields.io/badge/FastAPI-0.100+-green?style=for-the-badge&logo=fastapi)
![React](https://img.shields.io/badge/React-18+-61DAFB?style=for-the-badge&logo=react)
![Gemini](https://img.shields.io/badge/Gemini-AI-orange?style=for-the-badge&logo=google)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

> An intelligent, AI-powered auditing system that automatically audits enterprise systems, detects compliance gaps, generates evidence, and prepares audit documentation.

---

## 📌 Overview

**AI Enterprise Audit Agent** is a full-stack AI agent that automates the entire compliance auditing workflow for enterprises. It uses **Google Gemini AI**, **NLP**, and **Knowledge Graphs** to:

- 🔍 Automatically audit enterprise systems against compliance frameworks
- ⚠️ Detect compliance gaps in real-time
- 📑 Generate audit evidence automatically
- 🧠 Build a Knowledge Graph of assets, rules & relationships
- 📊 Produce professional audit reports (PDF/HTML)
- 🎨 Deliver insights via a modern React dashboard

Perfect for learning **AI agents**, **compliance automation**, and **full-stack AI projects**.

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| 🤖 **AI-Powered Auditing** | Gemini AI analyzes systems & finds compliance gaps |
| 📋 **Multi-Framework Support** | GDPR, ISO 27001, SOC 2, HIPAA, PCI-DSS |
| 🧠 **Knowledge Graph** | Visualizes relationships between assets, rules & risks |
| 📄 **Auto Evidence Generation** | AI creates audit evidence automatically |
| 📊 **Beautiful Dashboard** | Real-time charts, stats & activity feed |
| 📑 **Report Generator** | Export audit reports in PDF/HTML |
| 🔐 **JWT Authentication** | Secure login & role-based access |
| 🎯 **Gap Detection** | NLP-based gap analysis on policies & documents |
| 📤 **File Uploads** | Upload policies, logs & documents for audit |
| 🌙 **Modern UI** | Dark mode, glassmorphism, smooth animations |

---

## 🛠️ Tech Stack

### Backend
- **Python 3.10+**
- **FastAPI** – REST API framework
- **SQLAlchemy** – ORM
- **SQLite** – Database (practice-friendly, CPU-based)
- **Google Gemini API** – AI analysis
- **spaCy / NLTK** – NLP processing
- **NetworkX** – Knowledge Graph
- **ReportLab / WeasyPrint** – PDF generation
- **JWT (python-jose)** – Authentication
- **Pydantic** – Data validation

### Frontend
- **React 18** + **Vite**
- **TailwindCSS** – Styling
- **React Router v6** – Routing
- **Axios** – API calls
- **Recharts** – Charts & graphs
- **Framer Motion** – Animations
- **Lucide React** – Icons
- **React Hot Toast** – Notifications

### Database
- **SQLite** (easy setup, no server needed)

---

## 📂 Project Structure



---

## 🚀 Getting Started

### Prerequisites

- Python 3.10+
- Node.js 18+
- Google Gemini API Key ([Get one free](https://aistudio.google.com/apikey))
- Git

### 🔧 Backend Setup

```bash
# 1. Navigate to backend
cd backend

# 2. Create virtual environment
python -m venv venv

# 3. Activate it
# Windows:
venv\Scripts\activate
# macOS/Linux:
source venv/bin/activate

# 4. Install dependencies
pip install -r requirements.txt

# 5. Create .env file
cp .env.example .env
# Add your GEMINI_API_KEY in .env

# 6. Initialize database
python scripts/init_db.py

# 7. Seed demo data (optional)
python seed_data/seed_rules.py
python seed_data/seed_users.py

# 8. Run the server
uvicorn main:app --reload --port 8000


# 1. Navigate to frontend
cd frontend

# 2. Install dependencies
npm install

# 3. Create .env file
echo "VITE_API_URL=http://localhost:8000" > .env

# 4. Run dev server
npm run dev