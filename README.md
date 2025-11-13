# 🌐 ModelMatrix AI

### _AI Model Inventory • Marketplace • Management Platform_

ModelMatrix AI is a full-stack web application designed to manage,
explore, and purchase AI models.\
It features authentication, CRUD operations, secure private routes,
model purchasing, filtering, animations, and more --- all wrapped inside
a modern, elegant UI.

---

## 🚀 Live Links

Platform Link

---

🌍 **Live Client:** _[https://model-matrix-ai.netlify.app/]  
 🛠️ **Backend API:** _[https://modelmatrixapi.vercel.app/]

---

## ✨ Project Features

### 🔓 Public Features

- Browse all AI models
- Search and filter models (Framework, Dataset, Use-Case, Keyword)
- Beautiful responsive layout
- Light / Dark Theme (DaisyUI)
- Detailed model description pages
- Modern UI animations with Framer Motion

### 🔐 Authenticated Features

- Login & Register using Firebase Authentication
- Add new AI models (Create)
- Update existing models (Update)
- Delete models (Delete)
- View **My Models**
- View **My Purchases**
- Secure Protected Routes using PrivateRoute
- SweetAlert2 notifications
- Secure Axios interceptor with Firebase token

---

## 🛠️ Tech Stack

### Frontend

- ⚛️ React (Vite)
- 🎨 TailwindCSS + DaisyUI
- 💫 Framer Motion
- 🔥 Firebase Authentication
- ⚡ Axios + Secure Axios Hook
- 🍞 SweetAlert2 Notifications

### Backend

- 🚀 Express.js
- 🍃 MongoDB (Native Driver)
- 🔐 Firebase Admin Token Verification

---

## 📁 Folder Structure (Client)

    src/
     ├── Components/
     │   ├── Navbar/
     │   ├── Footer/
     │   ├── Pages/
     │   │   ├── Home/
     │   │   ├── Login/
     │   │   ├── Register/
     │   │   ├── AddModel/
     │   │   ├── UpdateModel/
     │   │   ├── ModelDetails/
     │   │   ├── AllModels/
     │   │   ├── MyModels/
     │   │   ├── MyPurchase/
     │   │   └── Error/
     │   └── Shared/
     │
     ├── hooks/
     │   ├── useAuth.js
     │   ├── useAxios.js
     │   └── useSecureAxios.js
     │
     ├── Context/
     │   └── AuthProvider.jsx
     │
     ├── Firebase/
     │   └── firebase.config.js
     │
     ├── Router/
     │   ├── Router.jsx
     │   └── PrivateRoute.jsx
     │
     └── main.jsx

---

## 🔐 Authentication Flow

1.  User signs in via Firebase.

2.  Firebase generates an ID Token.

3.  Secure Axios attaches this token in headers:

        Authorization: Bearer <token>

4.  Server verifies token using Firebase Admin SDK.

5.  Access granted to protected endpoints.

---

## 🧩 API Endpoints

### Models

Method Route Description

---

GET `/models` Get all models
GET `/models/:id` Get a model
POST `/models` Add model (protected)
PUT `/models/:id` Update model (protected)
DELETE `/models/:id` Delete model (protected)

### User Models

Method Route Description

---

GET `/my-models?email=...` User's added models

### Purchases

Method Route Description

---

POST `/purchase` Purchase a model
GET `/purchases?email=...` Purchased models

---

## 🌟 Pages Included

- **Home Page**
- **All Models Page** (Filters + Search + Sorting)
- **Model Details Page**
- **Add Model Page** _(Private)_
- **Update Model Page** _(Private)_
- **My Models Page** _(Private)_
- **My Purchases Page** _(Private)_
- **Login Page**
- **Register Page**
- **404 Error Page**
- **Loading Pages**

---

## 🖥️ Installation Guide

### 1️⃣ Clone the repo

    git clone https://github.com/your-repo-link
    cd modelmatrix-ai

### 2️⃣ Install dependencies

    npm install

### 3️⃣ Create `.env` file

    VITE_apiKey=xxxx
    VITE_authDomain=xxxx
    VITE_projectId=xxxx
    VITE_storageBucket=xxxx
    VITE_messagingSenderId=xxxx
    VITE_appId=xxxx

    VITE_API_URL=https://your-backend-url

### 4️⃣ Run the app

    npm run dev

---

## 🎨 UI Screenshots (Add yours)

    📌 Home Page
    📌 All Models
    📌 Model Details
    📌 Add Model
    📌 Update Model
    📌 My Models
    📌 My Purchases
    📌 Theme Toggle Demo

---

## 📦 Deployment

### Client:

- Firebase Hosting
- Netlify / Vercel (optional)

### Server:

- Vercel / Render / Railway

### Database:

- MongoDB Atlas

---

## 🙌 Final Notes

ModelMatrix AI is designed with: - Clean UI\

- Fast Performance\
- Modern Animations\
- Fully Protected Backend\
- Professional Architecture

If you want an **even more premium README** with screenshots included,
just share your images and I'll finalize it beautifully.

---

Made with ❤️ for your Assignment.
