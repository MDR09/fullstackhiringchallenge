# Full Stack Hiring Challenge - Manish Dharawaniya

## 🚀 Live Demo
https://smart-blog-editor-mdr.vercel.app/

## 📂 GitHub Repo
https://github.com/MDR09/Smart-Blog-Editor

## 🛠 Tech Stack
React, Node.js, Express, MongoDB

## ⚙ Setup Instructions

Backend Setup
# Navigate to backend directory
cd backend

# Create virtual environment
python -m venv venv

# Activate virtual environment
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Create .env file
cp .env.example .env
Configure backend/.env:

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
Start the backend server:

uvicorn app.main:app --reload --port 8000
Backend will run at: http://localhost:8000
API Documentation: http://localhost:8000/docs

Frontend Setup
# Navigate to frontend directory (from project root)
cd frontend

# Install dependencies
npm install

# Create .env file
cp .env.example .env
Configure frontend/.env:

VITE_API_URL=http://localhost:8000
Start the development server:

npm run dev

