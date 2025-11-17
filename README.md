#  Blog App – Deployment & DevOps 

This repository contains the deployed MERN Stack Blog Application for Week 7 of the Power Learn Project.  
The assignment focuses on deploying a full MERN application, configuring environment variables, implementing CI/CD, and setting up monitoring and maintenance.

---

##  Live Project Links

- 🌐 **Frontend (Vercel):**  
  [https://chatapp-frontend-stephen-oduors-projects.vercel.app](https://chatapp-frontend-stephen-oduors-projects.vercel.app)

- 🛠️ **Backend API (Render):**  
  [https://blogapp-backend-31p9.onrender.com](https://blogapp-backend-31p9.onrender.com)

---
## Screenshots
<img width="1127" height="792" alt="image" src="https://github.com/user-attachments/assets/61b64aae-1513-457f-b57a-9c62d1a79076" />

<img width="1113" height="783" alt="image" src="https://github.com/user-attachments/assets/f7dc26a4-0bd9-4c6b-8a69-ec192f255896" />




## 📌 Project Overview

This is a full-stack Blog Platform built with the MERN stack:

- **Frontend:** React + Vite
- **Backend:** Node.js + Express.js
- **Database:** MongoDB Atlas
- **Hosting:** Render (Backend), Vercel (Frontend)

### ✨ Key Features

- User Registration & Login
- JWT Authentication
- Secure Password Handling
- Production Environment Deployment

---

## 🧩 Tech Stack

| Layer        | Technology                     |
|--------------|--------------------------------|
| Frontend     | React, Vite, Tailwind CSS      |
| Backend      | Node.js, Express.js            |
| Database     | MongoDB Atlas                  |
| Authentication | JWT, bcrypt                 |
| Deployment (Backend) | Render                |
| Deployment (Frontend) | Vercel               |
| CI/CD        | GitHub Actions                 |

---

## 🎯Tasks Completed

### ✅ Task 1: Preparing the Application for Deployment

- Created production builds using Vite
- Configured environment variables (.env) for frontend & backend
- Implemented error handling in Express
- Enabled secure HTTP headers
- Connected to MongoDB Atlas (production cluster)
- Enabled database connection pooling

### 🚀 Task 2: Backend Deployment (Render)

- Created a Render Web Service
- Configured environment variables:
  - `MONGO_URI`
  - `JWT_SECRET`
  - `CLIENT_URL`
- Enabled automatic deployment from GitHub
- Set up CORS for frontend domain
- Render provides automatic SSL/HTTPS

### 🎨 Task 3: Frontend Deployment (Vercel)

- Connected GitHub repo to Vercel
- Added environment variable: `VITE_API_URL`
- Set build output directory: `dist`
- Enabled automatic deploys on `main` branch push
- Optimized production assets

### 🔄 Task 4: CI/CD Pipeline Setup

- Implemented GitHub Actions workflow:
  - Runs lint checks
  - Builds frontend & backend
  - Checks for compilation issues
  - Auto-deploys to Render and Vercel on successful build

### 📈 Task 5: Monitoring & Maintenance

#### Monitoring Tools

- Render Health Check Endpoint
- Vercel Deployment Logs
- MongoDB Atlas Performance Monitoring
- Backend server console logs

#### Maintenance Plan

- Regular dependency updates
- Database backups via MongoDB Atlas
- Documented rollback steps (revert commit & redeploy)
- Continuous monitoring via platform dashboards

---

## 📁 Environment Variables

### Backend `.env`

```env
MONGO_URI=your_mongo_atlas_url
JWT_SECRET=your_secret_key
CLIENT_URL=https://chatapp-frontend-stephen-oduors-projects.vercel.app

```

### Frontend `.env`
```
VITE_API_URL=https://blogapp-backend-31p9.onrender.com/
```
### 🛠️ Setup Instructions (Local Development)
#### Clone the repository
```
   git clone PLP-MERN-Stack-Development/deployment-and-devops-essentials-stephen-otieno.git
   cd blog-app
```
### Install backend packages
```
cd server
npm install

```

### - Install frontend packages
```
cd client
npm install
```
### Start development servers
#### Backend:
```
npm run dev
```

#### Frontend

```
npm run dev
```








