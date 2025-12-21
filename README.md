# Web_projects
NOVA AI – Intelligent Chat Assistant
NOVA AI is a full-stack AI-powered chat application built using modern web technologies. It provides real-time conversational responses using a large language model, with a clean UI and persistent chat storage.
This project demonstrates end-to-end AI application development, from frontend UI to backend APIs and database integration.
________________________________________
Features
•	Real-time AI chat responses
•	AI powered by Groq LLM
•	Dark / Light theme toggle
•	Fast REST API using Django
•	Chat history stored in MongoDB
•	Enter key support
•	Clean frontend–backend separation
________________________________________
Tech Stack
Frontend
•	HTML5
•	CSS3 
•	JavaScript (Fetch API)
Backend
•	Python 3
•	Django
•	Django REST Framework
AI Integration
•	Groq API (LLM-based chat completions)
Database
•	MongoDB
________________________________________
Project Structure
nova-ai/
│
├── backend/
│   ├── myworld/              # Virtual environment
│   └── nova_backend/
│       ├── chat/
│       │   ├── views.py
│       │   ├── ai_service.py
│       │   └── urls.py
│       ├── nova_backend/
│       │   ├── settings.py
│       │   ├── urls.py
│       │   └── manage.py
│
└── frontend/
    ├── index.html
    ├── style.css
    └── script.js
________________________________________
Setup & Installation
1. Clone the repository
git clone https://github.com/Giri-Nova/Web_projects.git
cd nova-ai 
________________________________________

2. Backend setup
Activate virtual environment
cd backend
myworld\Scripts\activate
Install dependencies
pip install -r requirements.txt
Run migrations
python manage.py migrate
Start Django server
python manage.py runserver
Backend will run at:
http://127.0.0.1:8000/
________________________________________
3. Frontend setup
•	Open frontend/index.html
•	Use Live Server (VS Code) or double-click the file
Frontend communicates with backend via REST API.
________________________________________
4. API Endpoint
Chat API
POST /api/chat/
Request body
{
  "message": "Hello NOVA"
}
Response
{
  "reply": "Hello! How can I help you today?"
}
________________________________________


How NOVA AI Works
1.	User enters a message in the frontend
2.	JavaScript sends the message to Django REST API
3.	Django calls Groq AI model
4.	AI response is returned
5.	Conversation is stored in MongoDB
6.	Response is displayed in UI
________________________________________
UI Features
•	Smooth message animations
•	Dark / Light theme toggle
•	Responsive layout
•	Typing indicator ("NOVA is thinking...")
________________________________________ Environment Variables
•	Create a .env file in backend directory:
•	GROQ_API_KEY=your_api_key_here
•	MONGO_URI=your_mongodb_uri
________________________________________
Status
•	Stable
•	Fully working
•	Version 1 completed
________________________________________
Future Enhancements
•	User authentication
•	Voice input/output
•	Chat history per user
•	Deployment to cloud
________________________________________
Author
Giri Manigandan M
B.E Computer Science and Engineering
Full Stack Developer | AI Enthusiast
________________________________________
Final Note
This project was built from scratch to understand real-world AI system design, API integration, and full-stack development practices.
Virtual environment not included. Use requirements.txt to install dependencies
________________________________________

