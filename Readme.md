# 🏫 School App - School Management System

[![React](https://img.shields.io/badge/React-19-blue?style=for-the-badge&logo=react)](https://reactjs.org/)
[![Node.js](https://img.shields.io/badge/Node.js-20-green?style=for-the-badge&logo=node.js)](https://nodejs.org/)
[![MongoDB](https://img.shields.io/badge/MongoDB-8-green?style=for-the-badge&logo=mongodb)](https://mongodb.com/)
[![Vercel](https://img.shields.io/badge/Vercel-Deploy-black?style=for-the-badge&logo=vercel)](https://vercel.com/)

## 📖 Overview
**School App** is a modern, full-stack **Progressive Web App (PWA)** for comprehensive school management. It provides role-based dashboards for admins, teachers, and students/parents with features like student enrollment, attendance tracking, test results, and secure authentication.

Built with best-in-class technologies, it's deployable to Vercel with zero configuration.

## ✨ Features
- 👥 **Role-based Authentication**: Admin, Teacher, Student/Parent logins with email verification, forgot password, and secure JWT tokens.
- 👨‍🎓 **Student Management**: Add, view all students, detailed profiles (Admin dashboard).
- 📊 **Attendance & Test Results**: Track attendance and manage exam scores.
- 📱 **PWA Support**: Installable app with offline capabilities (service worker).
- 📧 **Email Integration**: Verification and password reset emails.
- ☁️ **Cloudinary**: Image uploads for student profiles.
- 🚀 **Responsive Design**: TailwindCSS + DaisyUI for mobile-first UI.

## 🛠️ Tech Stack

| Frontend | Backend | Database | Tools |
|----------|---------|----------|-------|
| React 19 | Node.js + Express 5 | MongoDB + Mongoose 9 | Vite 7, TailwindCSS, DaisyUI |
| Zustand State | JWT + bcrypt |  | Vercel, Cloudinary |
| React Router v7 | Nodemailer |  | Axios, Framer Motion |

## 📸 Screenshots

### Authentication Flow
![Signup](screenshots/Screenshot%202026-03-19%20202315.png)
![Login](screenshots/Screenshot%202026-03-19%20202338.png)
![Email Verification](screenshots/Screenshot%202026-03-19%20202358.png)

### Dashboards
![Home Role Selection](screenshots/Screenshot%202026-03-19%2020415.png)
![Admin Dashboard](screenshots/Screenshot%202026-03-19%20203105.png)
![Teacher Dashboard](screenshots/Screenshot%202026-03-19%20203255.png)

### Student Management
![All Students](screenshots/Screenshot%202026-03-19%20203311.png)
![Add Student](screenshots/Screenshot%202026-03-19%20203359.png)
![Student Details](screenshots/Screenshot%202026-03-19%20203432.png)

### Other
![Test Results](screenshots/Screenshot%202026-03-19%20203542.png)
![Developer Profile](screenshots/Screenshot%202026-03-19%20203558.png)

## 📁 Project Structure
```
school/
├── frontend/           # React + Vite app
│   ├── src/
│   │   ├── pages/      # Auth, dashboards, student pages
│   │   ├── store/      # Zustand stores
│   │   └── config/     # School sections/subjects
│   └── public/
├── server/             # Node/Express API
│   ├── controllers/    # Business logic
│   ├── models/         # MongoDB schemas
│   ├── routers/        # API routes
│   └── utils/          # Email, tokens
├── screenshots/        # UI screenshots
├── Readme.md          # 📄 This file!
└── TODO.md            # Remaining tasks
```

## 🚀 Quick Start

### Prerequisites
- Node.js 20+
- MongoDB (Atlas or local)
- Accounts: Cloudinary, Resend/Nodemailer SMTP, MongoDB Atlas

### Backend Setup
```bash
cd server
npm install
# Copy .env.example to .env and configure:
# MONGO_URI=mongodb://...
# JWT_SECRET=your-secret
# CLOUDINARY_CLOUD_NAME=...
# RESEND_API_KEY=... (or SMTP)
npm run dev  # http://localhost:5000
```

### Frontend Setup
```bash
cd frontend
npm install
npm run dev  # http://localhost:5173
```

### Environment Variables (server/.env)
```
NODE_ENV=development
PORT=5000
MONGO_URI=your-mongodb-uri
JWT_SECRET=your-jwt-secret
COOKIE_EXPIRE=7
CLOUDINARY_CLOUD_NAME=...
CLOUDINARY_API_KEY=...
CLOUDINARY_API_SECRET=...
RESEND_API_KEY=...  # or SMTP_HOST, SMTP_PORT, etc.
```

## 🌐 Deployment
- **Frontend**: Deploy `frontend/` to Vercel (drag-drop or CLI).
- **Backend**: Deploy `server/` to Vercel (serverless functions).
- Both have `vercel.json` configured.

## 🔮 Future Features (see frontend/TODO.md)
- Real-time notifications (Socket.io present)
- Bulk import/export students
- Reports & analytics
- Parent portal enhancements

## 🤝 Contributing
1. Fork & clone
2. Create feature branch
3. `npm i` in frontend/server
4. Commit & PR

## 📄 License
MIT License - feel free to use/modify!

---

⭐ **Star the repo if you found it useful!** 👨‍💻 **Developed by [Developer](frontend/public/developer.jpeg)**
