# 🧠 BlogLens – AI-Powered Blog Application

**BlogLens** is a full-stack AI-powered blog application that allows users to **generate, edit, and manage blogs using OpenAI/Gemini**. It is built using the **MERN stack (MongoDB, Express.js, React, Node.js)**.


## 📌 Features

- 👤 User Authentication (Login / Signup via Clerk or JWT)
- 🧠 AI-powered blog generation (OpenAI / Gemini)
- 📝 Create, Edit, and Delete blogs
- 🖼️ Image upload and embedding (ImageKit / Cloudinary)
- 🔐 Secure backend with JWT / Clerk
- 💾 Persistent Redux state across refresh
- 📱 Fully responsive UI using TailwindCSS

---

## 🛠️ Tech Stack

**Frontend**
- React (Vite)
- Redux Toolkit & Redux Persist
- Axios
- TailwindCSS
- React Router
- Clerk (Auth)
- ImageKit / Cloudinary

**Backend**
- Node.js
- Express.js
- MongoDB (Mongoose)
- OpenAI / Gemini API
- JWT, bcrypt
- ImageKit SDK
- CORS, Cookie Parser

**Hosting**
- Frontend: Vercel  
- Backend: Render  
- Database: MongoDB Atlas

---

## 📁 Project Structure

### 📁 Frontend Folder Structure

```
client/
├── public/
│   └── index.html
├── src/
│   ├── assets/
│   ├── components/
│   ├── pages/
│   ├── redux/
│   ├── utils/
│   ├── App.jsx
│   └── main.jsx
├── .env
├── package.json
└── vite.config.js
```

### 📁 Backend Folder Structure

```
server/
├── config/
│   └── db.js
├── controllers/
│   ├── blogController.js
│   └── userController.js
├── middleware/
│   └── authMiddleware.js
├── models/
│   ├── blogModel.js
│   └── userModel.js
├── routes/
│   ├── blogRoutes.js
│   └── userRoutes.js
├── utils/
│   └── aiService.js
├── .env
├── index.js
└── package.json
```

---

## 🧑‍💻 Getting Started Locally

### 1. Clone the Repo

```bash
git clone https://github.com/amitkumar908/Blog-Lens-
cd bloglens
```

### 2. Setup Backend

```bash
cd server
npm install
```

Create `.env` in `/server`:

```
PORT=5000
MONGO_URI=your_mongodb_connection_string
OPENAI_API_KEY=your_openai_api_key
IMAGEKIT_PRIVATE_KEY=your_imagekit_private_key
IMAGEKIT_PUBLIC_KEY=your_imagekit_public_key
IMAGEKIT_URL_ENDPOINT=your_imagekit_url
JWT_SECRET=your_jwt_secret
FRONTEND_URL=http://localhost:5173
```

Start the backend:

```bash
npm run dev
```

### 3. Setup Frontend

```bash
cd ../client
npm install
```

Create `.env` in `/client`:

```
VITE_API_URL=http://localhost:5000/api
VITE_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
```

Start the frontend:

```bash
npm run dev
```

---

## 🔐 Environment Variables

### Backend `.env`

```
PORT=5000
MONGO_URI=your_mongodb_uri
OPENAI_API_KEY=your_openai_key
IMAGEKIT_PRIVATE_KEY=your_imagekit_private_key
IMAGEKIT_PUBLIC_KEY=your_imagekit_public_key
IMAGEKIT_URL_ENDPOINT=your_imagekit_url
JWT_SECRET=your_jwt_secret
FRONTEND_URL=http://localhost:5173
```

### Frontend `.env`

```
VITE_API_URL=http://localhost:5000/api
VITE_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
```

---

## ⚙️ Deployment

- **Frontend:** GitHub → Vercel (Auto Deploy)
- **Backend:** GitHub → Render (Auto Deploy)
- **Database:** MongoDB Atlas
- **Media Upload:** ImageKit or Cloudinary
- **AI API:** OpenAI or Gemini

---

## 🧠 Author

Made by ❤️ by [Amit Kumar Bhorayat](https://github.com/amitkumar908)

---

## 📃 License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.
