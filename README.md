🧠 Immersive LMS (Backend API)
This is the backend for the Immersive Learning Management System, designed to deliver spiritually inspired, multimedia-rich educational experiences.

Built with FastAPI, it provides:

📚 GET /courses – Lists available course modules

💬 POST /chat – Sends user prompts to GPT-4 and returns AI-generated responses

🚀 Setup Instructions
1. Clone this repository

git clone https://github.com/michaellawrencemorgan/LMS-Test.git
cd LMS-Test

2. Install dependencies

pip install -r requirements.txt

3. Create your .env file
In the project root, add:

OPENAI_API_KEY=your-openai-key-here

4. 🏃‍♂️ Run the Backend Server

uvicorn main:app --reload
Visit: http://localhost:8000/docs to interact with the API via Swagger UI.

5. 🧪 Example API Usage
GET /courses
Returns structured modules like this:

[
  {
    "course_id": "prophetic_matrix",
    "title": "The Prophetic Matrix",
    "modules": [
      {
        "title": "Module 1: Revelation",
        "content": "Video + PDF + Prompt",
        "quiz": {
          "question": "...",
          "answer": "..."
        }
      }
    ]
  }
]
POST /chat
Request:

{
  "prompt": "What does it mean to walk by faith?"
}
Response:

json
Copy
Edit
{
  "reply": "To walk by faith means to trust in divine guidance beyond visible evidence..."
}

6. 📦 Tech Stack
FastAPI – Web API framework

OpenAI – GPT-4 conversational intelligence

dotenv – Secure API key loading

uvicorn – ASGI server for local dev

7. ✅ Roadmap Ideas
Add user authentication

Expand course content structure

Include audio/visual response integration

Connect to a frontend (React or VR)
