# Full Stack Hiring Challenge - Manish Dharawaniya

## 🚀 Live Demo
https://smart-blog-editor-mdr.vercel.app/

## 📂 GitHub Repository
https://github.com/MDR09/Smart-Blog-Editor

---

## 🛠 Tech Stack

- React (Frontend)
- FastAPI (Backend)
- MongoDB
- JWT Authentication
- Google Gemini API

---

# ⚙ Setup Instructions

## 🔹 Backend Setup

Navigate to backend directory:

```bash
cd backend
```

Create virtual environment:

```bash
python -m venv venv
```

Activate virtual environment:

Windows:
```bash
venv\Scripts\activate
```

macOS/Linux:
```bash
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Create `.env` file:

```bash
cp .env.example .env
```

Configure `backend/.env`:

```env
# MongoDB Configuration
MONGODB_URL=mongodb+srv://username:password@cluster0.mongodb.net/?appName=Cluster0
DATABASE_NAME=smart_blog_editor

# JWT Configuration
SECRET_KEY=your-super-secret-key-change-this-in-production
ALGORITHM=HS256
ACCESS_TOKEN_EXPIRE_MINUTES=1440

# Google Gemini API Key
GEMINI_API_KEY=your-gemini-api-key-here

# Environment
ENVIRONMENT=development
```

Start backend server:

```bash
uvicorn app.main:app --reload --port 8000
```

Backend runs at:
http://localhost:8000

API Docs:
http://localhost:8000/docs

---

## 🔹 Frontend Setup

Navigate to frontend directory:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Create `.env` file:

```bash
cp .env.example .env
```

Configure `frontend/.env`:

```env
VITE_API_URL=http://localhost:8000
```

Start development server:

```bash
npm run dev
```

---

## 👨‍💻 Author

**Manish Dharawaniya**  
GitHub: https://github.com/MDR09  
Live Project: https://smart-blog-editor-mdr.vercel.app/
