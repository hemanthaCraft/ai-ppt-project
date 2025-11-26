🌟 AI Document Generator


A fast and intelligent platform that helps you generate, refine, and export professional Word documents and PowerPoint presentations using AI.
Designed for students, working professionals, and creators who need high-quality content in seconds.

🚀 Live Demo

👉 Add your deployed link here (Frontend on Vercel + Backend on Render)

✨ Features
🤖 AI Content Creation

Generate full document sections using Gemini AI from just a topic or short prompt.

✏️ Smart Editing

Refine content with natural commands:

“Make it formal”

“Shorten it”

“Rewrite in bullet points”

📤 Export to Office

Download ready-to-use .docx and .pptx files.

📁 Project Management

Save, edit, update, and revisit multiple drafts.

👍 Interactive Controls

Like, dislike, or comment on AI-generated sections.

🔐 Secure Authentication

Uses Firebase Auth for login/signup.

🛠️ Tech Stack

Frontend: React, Vite, Firebase
Backend: FastAPI, Python
AI Model: Gemini API
Database: Firebase Firestore
Hosting: Vercel (Frontend), Render (Backend)

📦 Project Structure
AI-Document-Generator/
├── backend/
│   ├── main.py
│   ├── requirements.txt
│   ├── .env
│   └── utils/
│       ├── docx_generator.py
│       └── pptx_generator.py
└── frontend/
    ├── src/
    │   ├── pages/
    │   ├── components/
    │   ├── firebase.js
    │   └── config.js
    └── package.json

🧩 Setup & Installation
1️⃣ Clone the Repository
git clone https://github.com/YOUR_USERNAME/AI-Document-Generator.git
cd AI-Document-Generator

⚙️ Backend Setup
Create virtual environment:
cd backend
python -m venv venv

Activate:
venv\Scripts\activate       # Windows
source venv/bin/activate    # macOS / Linux

Install packages:
pip install -r requirements.txt

Add .env file:
GEMINI_API_KEY=your_key_here

Start server:
python main.py


Backend runs on:
👉 http://localhost:8000

🌐 Frontend Setup
cd frontend
npm install

Configure Firebase

Edit:

src/firebase.js

Add backend URL

Edit:

src/config.js

Run frontend:
npm run dev


Frontend runs on:
👉 http://localhost:5173

🌉 Architecture
User → React Frontend → FastAPI Backend → Gemini AI
                       ↓
                 Firebase Firestore

📡 API Endpoints
Method	Endpoint	Description
POST	/api/generate-section	Generate AI content
POST	/api/refine-section	Improve/refine content
POST	/api/export-document	Export docx/pptx file

Swagger UI available at:
👉 http://localhost:8000/docs

🚀 Deploying
Backend — Render

Root: backend/

Build: pip install -r requirements.txt

Start:

uvicorn main:app --host 0.0.0.0 --port $PORT


Add env: GEMINI_API_KEY

Frontend — Vercel

Root: frontend/

Build: npm run build

Output: dist

Update backend URL in config.js

🐞 Troubleshooting

Backend not starting?
✔ Install dependencies
✔ Check .env
✔ Python 3.11 required

Frontend not loading?
✔ Wrong backend URL
✔ Firebase config missing

Export failing?
✔ Ensure python-docx & python-pptx installed
✔ Check backend logs

📄 License

Licensed under the MIT License.

⭐ Support

If you like this project, consider giving it a star ⭐ on GitHub!
