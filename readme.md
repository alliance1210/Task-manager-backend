# Task Manager API

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [API Documentation](#api-documentation)
- [Environment Variables](#environment-variables)

## Features
- 🔐 JWT-based Authentication & Authorization
- ✅ CRUD Operations for Tasks
- 🚀 RESTful API Design
- 🌐 CORS Support

## Installation


1. **Clone the repository**
```bash
git clone https://github.com/alliance1210/Task-manager-backend.git
cd task-manager-backend
```

2. **Install dependencies**
```bash
npm install
```

3. **Set up environment variables**
Create .env file in root directory:
```bash
MONGODB_URI=your_mongodb_atlas_connection_string
JWT_SECRET=your_jwt_secret_key
PORT=5000
RATE_LIMIT_WINDOW=15
RATE_LIMIT_MAX=100
```

4. **Start the development server**
```bash
npm run dev
```

## API Documentation
Base URL
http://localhost:5000/

Example Endpoints

Method	Endpoint	    Description	       Authentication
POST	/auth/register	Register new user	Public
POST	/auth/login	    User login	        Public
GET	    /tasks	        Get all tasks	    Private
POST	/tasks	        Create new task	    Private
GET	    /tasks/:id	    Get single task	    Private
PUT	    /tasks/:id	    Update task	        Private
DELETE	/tasks/:id	    Delete task	        Private


## Environment Variables
Variable	 Description	                    Example
MONGODB_URI	 MongoDB Atlas connection string	mongodb+srv://user:pass@cluster...
JWT_SECRET	 Secret key for JWT signing	        supersecretkey123!
PORT	     Server port	                    5000