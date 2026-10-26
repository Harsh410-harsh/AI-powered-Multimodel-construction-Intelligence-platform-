# 🏗️ BuildMind — AI-Powered Multimodal Construction Intelligence Platform

**Build smarter. Build safer. Build with confidence.**

BuildMind is an intelligent construction decision-support platform designed to help construction professionals analyze site conditions, identify potential safety hazards, assess visible cracks, plan projects, evaluate property values, and access construction-related assistance through a unified workspace.

## 🚀 Live Demo

🌐 **Live Website:** https://ai-powered-multimodel-construction.vercel.app

🔗 **GitHub Repository:** https://github.com/Harsh410-harsh/AI-powered-Multimodel-construction-Intelligence-platform-

⚙️ **Backend API:** https://ai-powered-multimodel-construction.onrender.com

📚 **API Documentation:** https://ai-powered-multimodel-construction.onrender.com/docs

## 📌 Project Overview

BuildMind combines construction-related information, site images, and project details into a single decision-support workspace. Its goal is to make construction workflows more accessible, organized, and efficient.

The platform includes a web-based frontend and a Python backend API, with AI-powered capabilities depending on the configured AI provider and credentials.

## ✨ Key Features

- **Site Safety Analysis:** Review construction site conditions and potential safety hazards.
- **Crack Analysis:** Examine visible cracks and identify conditions that may require further inspection.
- **Project Planning:** Create preliminary project schedules and estimates.
- **Property Valuation:** Support preliminary property valuation workflows.
- **Site Assistant:** Access construction-related question-and-answer assistance.
- **Weather Advisory:** Provide weather-related information for construction planning.
- **Analysis History:** Access previous analyses where persistence is configured.
- **Decision Support Dashboard:** Manage construction tools through a unified interface.

> **Note:** AI-generated assessments are decision-support outputs, not substitutes for qualified structural engineers, safety professionals, or certified property valuers. Availability and accuracy depend on the implementation, configured services, and input data.

## 🛠️ Technology Stack

### Frontend
- React
- Vite
- JavaScript
- CSS

### Backend
- Python
- FastAPI
- Uvicorn
- Pydantic

### Deployment
- **Frontend:** Vercel
- **Backend:** Render
- **Version Control:** Git and GitHub

## 🏛️ System Architecture

```text
                   User
                    |
                    v
          React + Vite Frontend
                  (Vercel)
                    |
                    | HTTPS API Requests
                    v
             FastAPI Backend
                 (Render)
                    |
                    v
       Construction Analysis Services
                    |
                    v
          Results to the Frontend
```

## 🌐 Deployment Links

| Component | URL |
|---|---|
| Live Website | https://ai-powered-multimodel-construction.vercel.app |
| GitHub Repository | https://github.com/Harsh410-harsh/AI-powered-Multimodel-construction-Intelligence-platform- |
| Backend API | https://ai-powered-multimodel-construction.onrender.com |
| API Documentation | https://ai-powered-multimodel-construction.onrender.com/docs |

## ⚙️ Environment Configuration

### Frontend

Configure the following environment variable in Vercel:

```env
VITE_API_BASE_URL=https://ai-powered-multimodel-construction.onrender.com
```

For local development, create a `.env` file inside the frontend directory and set the API URL appropriate for your local backend.

### Backend

Configure the backend environment variables in Render according to your project's configuration and the provided `.env.example` file.

For cross-origin requests, configure:

```env
CORS_ORIGINS=http://localhost:5173,http://127.0.0.1:5173,https://ai-powered-multimodel-construction.vercel.app
```

Add any required AI provider credentials through your hosting provider's environment settings. Never commit API keys, passwords, or secret credentials to GitHub.

## 💻 Run Locally

### Prerequisites

- Python
- Node.js and npm
- Git

### 1. Clone the Repository

```bash
git clone https://github.com/Harsh410-harsh/AI-powered-Multimodel-construction-Intelligence-platform-.git
cd AI-powered-Multimodel-construction-Intelligence-platform-
```

### 2. Set Up the Backend

Create and activate a Python virtual environment from the project root.

**Windows PowerShell:**

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
```

Install backend dependencies:

```powershell
pip install -r backend/requirements.txt
```

Create your local environment file using the example configuration if needed, then start the API:

```powershell
cd backend
uvicorn app.main:app --reload
```

The backend should be available at:

http://127.0.0.1:8000

API documentation:

http://127.0.0.1:8000/docs

### 3. Set Up the Frontend

Open a second terminal from the project root:

```powershell
cd frontend
npm install
```

Create a `.env` file in the `frontend` directory:

```env
VITE_API_BASE_URL=http://127.0.0.1:8000
```

Start the frontend development server:

```powershell
npm run dev
```

Open the local URL displayed in your terminal, usually:

http://localhost:5173

## 📁 Project Structure

```text
multimodal-construction-intelligence/
├── backend/
│   ├── app/
│   │   ├── main.py
│   │   └── config.py
│   ├── requirements.txt
│   └── .env.example
├── frontend/
│   ├── src/
│   │   └── App.jsx
│   ├── package.json
│   └── .env.example
├── README.md
└── .gitignore
```

*The structure above highlights the main files discussed in the setup instructions; additional files and folders may exist in the repository.*

## 🔒 Security

- Keep API keys and secrets in environment variables.
- Do not upload `.env` files containing real credentials.
- Use `.gitignore` to exclude virtual environments, dependencies, caches, and secret files.
- Configure CORS to allow only the frontend origins you trust.

## 🚧 Current Status

The frontend and backend have been deployed separately using Vercel and Render.

Some AI capabilities may operate in demo mode until the required AI provider credentials and services are configured. Actual feature availability depends on backend configuration.

## 🔮 Future Improvements

- Advanced multimodal image analysis.
- Improved construction risk assessment.
- More detailed project scheduling and cost estimation.
- Persistent project and analysis history.
- User authentication and project management.
- Enhanced reporting and visualization.
- Integration with additional construction data sources.

## 🤝 Contributing

Contributions, suggestions, and bug reports are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Push the branch to your fork.
5. Open a pull request.

## 📄 License

Add a license file to the repository before specifying reuse or distribution permissions. Until a license is added, the project should be treated as having no explicit open-source license.

---

**BuildMind — Building a smarter, safer future through construction intelligence.**
