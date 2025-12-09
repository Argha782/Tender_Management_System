# ⚡ Tender Management System (MERN – Monorepo)

🔗 **Repository:** https://github.com/Argha782/Tender_Management_System  

🌐 **Frontend (Vercel):**  
- https://tms-argha-sahas-projects.vercel.app  
- https://tms-umber-phi.vercel.app  

🔌 **Backend API (Render):**  
- https://tender-management-system-nu1j.onrender.com  

---

## 📖 Overview

The **Tender Management System** is a full-stack **MERN application** designed to digitize the complete tender lifecycle.

It provides **role-based access** and workflow management for:
- 🧑‍💼 **Super Admin** – full platform control  
- 🏗️ **Tender Owners (Admins)** – manage their own tenders  
- 👷 **Vendors / Bidders** – view tenders, receive notifications, and place bids  

This project was developed as part of an **industry-oriented system** with secure authentication, document handling, and scalable deployment.

---

## 🏗️ Monorepo Structure

```text
Tender_Management_System/
├── frontend/        # React + Vite frontend (Vercel)
│   ├── src/
│   ├── public/
│   ├── .env
│   └── package.json
│
├── backend/         # Node + Express backend (Render)
│   ├── controllers/
│   ├── routes/
│   ├── models/
│   ├── middlewares/
│   ├── utils/
│   ├── public/
│   ├── index.js
│   └── package.json
│
└── README.md
```

---

## 🛠️ Tech Stack

### Frontend
- React.js
- Vite
- Tailwind CSS
- Headless UI
- Axios
- React Router DOM
- Context API / LocalStorage

### Backend
- Node.js
- Express.js
- MongoDB + Mongoose
- JWT Authentication
- Cloudinary
- Multer
- CORS

### Deployment
- Frontend: Vercel  
- Backend: Render  

---

## 🔐 Features

### ✅ Authentication & Roles
- JWT-based authentication
- Role-based access control
- Secure protected routes

### ✅ Tender Management
- Create, update, delete tenders
- Tender status tracking
- Tender filtering & search

### ✅ Notifications
- Role-based notifications
- System and tender-related alerts

### ✅ File Handling
- Secure document upload using Cloudinary
- Multiple document support per tender

---

## ⚙️ Local Setup Instructions

### 1️⃣ Clone the repository
```bash
git clone https://github.com/Argha782/Tender_Management_System.git
cd Tender_Management_System
```

---

## ▶️ Frontend Setup

```bash
cd frontend
npm install
```

Create a `.env` file inside `frontend/`:
```env
VITE_API_URL=http://localhost:5000
```

Start frontend:
```bash
npm run dev
```

📍 Runs on: http://localhost:5173

---

## ▶️ Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file inside `backend/`:
```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret

CLOUDINARY_CLOUD_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
```

Start backend:
```bash
npm run dev
```

📍 Runs on: http://localhost:5000

---

## 🌍 Deployment Details

### Frontend (Vercel)
- Root Directory: frontend
- Environment Variable:
```env
VITE_API_URL=https://tender-management-system-nu1j.onrender.com
```

### Backend (Render)
- Root Directory: backend
- Public API:
https://tender-management-system-nu1j.onrender.com

---

## ✅ CORS Configuration (Backend)

The backend allows requests from deployed frontend domains:
```js
origin: [
  "http://localhost:5173",
  "https://tms-argha-sahas-projects.vercel.app",
  "https://tms-umber-phi.vercel.app",
  /\.vercel\.app$/,
]
```

---

## 👨‍💻 Author

**Argha Saha**  
🎓 Master of Computer Applications (MCA)  
📧 Email: arghasaha782@gmail.com  
🔗 LinkedIn: https://www.linkedin.com/in/argha-saha-80527a208/

---

## 📌 Notes for Recruiters

- Monorepo architecture  
- Production-ready deployment  
- Secure JWT authentication  
- Cloudinary-based file uploads  
- Role-based system design  
