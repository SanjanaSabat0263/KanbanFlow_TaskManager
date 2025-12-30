# 🗂️ KanbanFlow Task Manager (MERN Stack)

KanbanFlow is a full-stack task management application inspired by tools like **Trello** and **Asana**.  
It helps users organize, track, and manage tasks efficiently using a **Kanban-style workflow**, with secure authentication and full CRUD functionality.

This project is developed as **Project 2 (Month 2)** of an internship program and follows a **documentation-driven, API-first development approach**.

---

## 🎯 Purpose

The purpose of the KanbanFlow Task Manager is to provide a secure and user-friendly platform for managing tasks using a Kanban workflow, while demonstrating real-world **full-stack MERN application development** skills.

---

## 🚀 Features

### 🔐 User Authentication
- User Registration
- User Login
- JWT-based authentication
- Protected API routes

### ✅ Task Management
- Create, Read, Update, Delete (CRUD) tasks
- Tasks are user-specific and secured

### 🔄 Kanban Workflow
- Task statuses:
  - To-Do
  - In-Progress
  - Completed
- Update task status directly from the UI

---

## 🛠️ Tech Stack

### Frontend
- React.js
- Axios
- React Router
- Context API (Global State Management)

### Backend
- Node.js
- Express.js
- MongoDB Atlas
- Mongoose
- bcrypt
- jsonwebtoken (JWT)

### Tools & Platforms
- Postman (API testing)
- Swagger (API documentation)
- Concurrently
- Render (Backend deployment)
- Vercel (Frontend deployment)
- Git & GitHub

---
Layer,Technology
Frontend,"React.js, Axios, React Router, Context API"
Backend,"Node.js, Express.js"
Database,"MongoDB Atlas, Mongoose"
Security,"Bcrypt (Hashing), JWT (Auth)"
Dev Tools,"Postman, Swagger, Concurrently, Git"
Deployment,"Render (Backend), Vercel (Frontend)"

## 📁 Project Structure (Monorepo)

kanbanflow-task-manager/
├── backend/
│   ├── config/         # Database connection (db.js)
│   ├── controllers/    # Logic for Auth and Task routes
│   ├── middleware/     # Auth middleware (JWT verification)
│   ├── models/         # Mongoose Schemas (User, Task)
│   ├── routes/         # API Endpoints
│   └── server.js       # Entry point
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/ # Reusable UI components (Navbar, Board, Card)
│   │   ├── context/    # Global State (AuthContext, TaskContext)
│   │   ├── pages/      # Login, Register, Dashboard
│   │   └── services/   # Axios API calls
│   └── App.js
└── package.json        # Root package for Concurrently scripts


⚙️ Installation & Setup
Clone the repository:

Bash

git clone https://github.com/your-username/kanbanflow.git
cd kanbanflow
Install dependencies for both Frontend and Backend:

Bash

# Root directory
npm install
# Backend directory
cd backend && npm install
# Frontend directory
cd ../frontend && npm install
Environment Variables: Create a .env file in the backend folder:

Code snippet

PORT=5000
MONGO_URI=your_mongodb_atlas_uri
JWT_SECRET=your_secret_key
Run the application: From the root directory, use concurrently to start both servers:

Bash

npm run dev
📝 API Documentation
The API follows a RESTful structure. Detailed documentation can be found via:

Swagger: Accessible at /api-docs when the server is running.

Postman: [Link to your Postman Collection if available]

🤝 Contributing
Fork the Project

Create your Feature Branch (git checkout -b feature/AmazingFeature)

Commit your Changes (git commit -m 'Add some AmazingFeature')

Push to the Branch (git push origin feature/AmazingFeature)

Open a Pull Request




