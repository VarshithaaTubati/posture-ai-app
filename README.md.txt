Posture AI Detection App

A full-stack web application that detects bad posture using rule-based logic in real time or from uploaded videos.

🔗 Deployed Links

🔵Frontend (React): [https://posture-ai-frontend.netlify.app](https://posture-ai-frontend.netlify.app)
🔵Backend (FastAPI): [https://posture-ai-backend.onrender.com](https://posture-ai-backend.onrender.com)
🎥Demo Video:(https://www.canva.com/design/DAGs1Mjr-9k/FjfBkKtuO4d53Yd3LZNMbg/watch?utm_content=DAGs1Mjr-9k&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=hf1e44536ac)


⚠️ IMPORTANT NOTE

> The backend is hosted on Render (Free Tier) which has a memory limit of **512MB**.  
> When overloaded, it may show errors like:  
> Ran out of memory (used over 512MB)` or cause delay in responses.

💡 How to test locally if backend crashes:

If backend link fails or gives `Network Error` in console:

1. Open the `frontend/src/App.js` file.
2. **Replace API endpoints** with these local ones:
    ```js
    axios.post("http://localhost:8000/analyze_webcam", ...)
    axios.post("http://localhost:8000/analyze", ...)
    ```

💻 Tech Stack

| Layer     | Tech Used                   |
|-----------|-----------------------------|
| Frontend  | React.js, Axios, HTML5 Video/Webcam |
| Backend   | FastAPI, OpenCV, MediaPipe, NumPy   |
| Deployment | Netlify (frontend), Render (backend) |


⚙️ Local Setup Instructions

➤ Step 1: Clone Repo

git clone https://github.com/VarshithaaTubati/posture-ai-app.git
cd posture-ai-app

➤ Step 2: Run Backend (FastAPI)

cd backend
pip install -r requirements.txt
uvicorn main:app --reload
🔗 Backend will run at: http://localhost:8000

➤ Step 3: Run Frontend (React)

cd ../frontend
npm install
npm install axios react-webcam
npm start
🔗 Frontend will run at: http://localhost:3000

✅ Features
Upload video or use webcam.
Detects bad posture:
⚠️ Knee over toe (squat)
⚠️ Back angle < 150°
⚠️ Neck bend > 30°
Returns live feedback + score.

📂 Folder Structure

posture-ai-app/
├── backend/
│   ├── main.py
│   └── requirements.txt
├── frontend/
│   ├── src/
│   ├── public/
│   └── App.js, index.js, etc.
└── README.md

🏁 Final Submission Checklist
✅ GitHub Repo: https://github.com/VarshithaaTubati/posture-ai-app

✅ Frontend: https://posture-ai-frontend.netlify.app

✅ Backend: https://posture-ai-backend.onrender.com

✅ Demo Video: https://www.canva.com/design/DAGs1Mjr-9k/FjfBkKtuO4d53Yd3LZNMbg/watch?utm_content=DAGs1Mjr-9k&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=hf1e44536ac

