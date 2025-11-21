# 💬 Real-Time Chat Application

<p align="center">
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB"/>
  <img src="https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white" alt="Express"/>
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React"/>
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white" alt="Node.js"/>
  <img src="https://img.shields.io/badge/Socket.io-010101?style=for-the-badge&logo=socket.io&logoColor=white" alt="Socket.io"/>
  <img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge" alt="License"/>
</p>

<p align="center">
  <b>A full-stack real-time chat application with instant messaging, online status, and beautiful UI ⚡</b>
</p>

<p align="center">
  <a href="#-installation">📦 Installation</a> •
  <a href="#-features">✨ Features</a> •
  <a href="#-tech-stack">🛠️ Tech Stack</a> •
  <a href="#-deployment">🚀 Deployment</a>
</p>

---

## 📋 Table of Contents

- [Problem Statement](#-problem-statement)
- [Solution](#-solution)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Tools Used](#-tools-used)
- [Installation](#-installation)
- [Environment Variables](#-environment-variables)
- [Deployment](#-deployment)
- [Future Scope](#-future-scope)
- [Contributing](#-contributing)
- [License](#-license)

---

## ❓ Problem Statement

Building a real-time communication platform involves several complex challenges:

- ⚡ **Real-Time Delivery** — Messages need to be delivered instantly without page refresh
- 🔐 **Security** — User authentication and message privacy are critical
- 🟢 **Presence System** — Users want to know who's online and available
- 📱 **Responsive Design** — Chat apps must work seamlessly across all devices
- 🔄 **State Synchronization** — Keeping UI in sync with real-time events is complex
- 🐛 **Error Handling** — Network issues and errors need graceful handling
- 💾 **Message Persistence** — Chat history must be stored and retrieved efficiently

---

## 💡 Solution

**Real-Time Chat App** is a full-stack messaging platform built with the MERN stack and Socket.io, delivering instant communication with a modern, responsive interface.

### ✨ Highlights

| Feature | Description |
|---------|-------------|
| 🌟 **MERN + Socket.io** | Full-stack real-time architecture |
| 🎃 **JWT Authentication** | Secure login with token-based auth |
| 👾 **Real-Time Messaging** | Instant message delivery with Socket.io |
| 🚀 **Online Status** | See who's online in real-time |
| 👌 **Zustand State** | Lightweight global state management |
| 🐞 **Error Handling** | Robust error handling on client & server |
| 🎨 **Beautiful UI** | TailwindCSS + DaisyUI for stunning design |
| ⭐ **Free Deployment** | Deploy like a pro at zero cost |

---

## ✨ Features

### 🔐 Authentication & Security

| Feature | Description |
|---------|-------------|
| 📝 **User Registration** | Sign up with email and password |
| 🔑 **Secure Login** | JWT-based authentication |
| 🛡️ **Protected Routes** | Authorization middleware |
| 🔒 **Password Hashing** | Bcrypt encryption |
| 🚪 **Logout** | Secure session termination |

### 💬 Messaging

| Feature | Description |
|---------|-------------|
| ⚡ **Real-Time Chat** | Instant message delivery via Socket.io |
| 🟢 **Online Status** | Live user presence indicators |
| 📜 **Chat History** | Persistent message storage |
| 👥 **User List** | Browse and select users to chat |
| 🔔 **Message Notifications** | Real-time message alerts |

### 🎨 User Experience

| Feature | Description |
|---------|-------------|
| 📱 **Responsive Design** | Works on desktop, tablet, and mobile |
| 🌙 **Modern UI** | Clean interface with DaisyUI components |
| ⚡ **Fast Performance** | Optimized React rendering |
| 🔄 **Live Updates** | UI syncs automatically with events |

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────────────────┐
│                    🌐 Frontend (React + Zustand)                │
│  ┌──────────────┐  ┌──────────────┐  ┌────────────────────────┐ │
│  │   Auth UI    │  │   Chat UI    │  │   Online Users Panel   │ │
│  │  (Login/     │  │  (Messages,  │  │   (Real-time status)   │ │
│  │   Signup)    │  │   Input)     │  │                        │ │
│  └──────────────┘  └──────────────┘  └────────────────────────┘ │
└─────────────────────────────┬───────────────────────────────────┘
                              │
                    ┌─────────┴─────────┐
                    │  HTTP    WebSocket │
                    │  (REST)  (Socket.io)│
                    └─────────┬─────────┘
                              │
┌─────────────────────────────┴───────────────────────────────────┐
│                 🔌 Backend (Node.js + Express)                  │
│  ┌──────────────┐  ┌──────────────┐  ┌────────────────────────┐ │
│  │  Auth Routes │  │ Message      │  │   Socket.io Server     │ │
│  │  (JWT)       │  │ Routes       │  │   (Real-time events)   │ │
│  └──────────────┘  └──────────────┘  └────────────────────────┘ │
└─────────────────────────────┬───────────────────────────────────┘
                              │
                              ▼
                    ┌─────────────────┐
                    │    MongoDB      │
                    │   (Database)    │
                    └─────────────────┘
```

---

## 🛠️ Tech Stack

### Frontend

| Technology | Purpose |
|------------|---------|
| ![React](https://img.shields.io/badge/React-61DAFB?style=flat&logo=react&logoColor=black) | User Interface |
| ![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white) | Styling |
| ![DaisyUI](https://img.shields.io/badge/DaisyUI-5A0EF8?style=flat&logo=daisyui&logoColor=white) | UI Components |
| ![Zustand](https://img.shields.io/badge/Zustand-433E38?style=flat) | State Management |
| ![Socket.io Client](https://img.shields.io/badge/Socket.io-010101?style=flat&logo=socket.io&logoColor=white) | Real-time Client |

### Backend

| Technology | Purpose |
|------------|---------|
| ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat&logo=node.js&logoColor=white) | Runtime Environment |
| ![Express](https://img.shields.io/badge/Express.js-000000?style=flat&logo=express&logoColor=white) | Web Framework |
| ![Socket.io](https://img.shields.io/badge/Socket.io-010101?style=flat&logo=socket.io&logoColor=white) | Real-time Server |
| ![JWT](https://img.shields.io/badge/JWT-000000?style=flat&logo=json-web-tokens&logoColor=white) | Authentication |

### Database

| Technology | Purpose |
|------------|---------|
| ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat&logo=mongodb&logoColor=white) | Database |
| ![Mongoose](https://img.shields.io/badge/Mongoose-880000?style=flat) | ODM |

---

## 🔧 Tools Used

| Tool | Purpose |
|------|---------|
| ![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white) | Version Control |
| ![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=flat&logo=visual-studio-code&logoColor=white) | IDE |
| ![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat&logo=postman&logoColor=white) | API Testing |
| ![MongoDB Compass](https://img.shields.io/badge/MongoDB_Compass-47A248?style=flat&logo=mongodb&logoColor=white) | Database GUI |
| ![npm](https://img.shields.io/badge/npm-CB3837?style=flat&logo=npm&logoColor=white) | Package Manager |

---

## 📦 Installation

### Prerequisites

- Node.js 18+
- MongoDB (local or Atlas)
- npm or yarn

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/armaan-arora/chat-app.git
cd chat-app
```

### 2️⃣ Install Dependencies

```bash
# Install backend dependencies
cd backend
npm install

# Install frontend dependencies
cd ../frontend
npm install
```

### 3️⃣ Set Up Environment Variables

Create `.env` file in the `backend` folder:

```env
PORT=5000
MONGODB_URI=mongodb://localhost:27017/chat-app
JWT_SECRET=your_super_secret_jwt_key
NODE_ENV=development
```

### 4️⃣ Run the Application

```bash
# Terminal 1 - Start backend
cd backend
npm run dev

# Terminal 2 - Start frontend
cd frontend
npm run dev
```

### 5️⃣ Access the App

- 🌐 **Frontend:** http://localhost:5173
- 🔌 **Backend:** http://localhost:5000

---

## 🔐 Environment Variables

| Variable | Description | Example |
|----------|-------------|---------|
| `PORT` | Backend server port | `5000` |
| `MONGODB_URI` | MongoDB connection string | `mongodb://localhost:27017/chat-app` |
| `JWT_SECRET` | Secret key for JWT tokens | `your_super_secret_key` |
| `NODE_ENV` | Environment mode | `development` or `production` |

---

## 📁 Project Structure

```
chat-app/
├── 📂 backend/
│   ├── 📂 config/
│   │   └── db.js                 # Database connection
│   ├── 📂 controllers/
│   │   ├── authController.js     # Auth logic
│   │   └── messageController.js  # Message logic
│   ├── 📂 middleware/
│   │   └── authMiddleware.js     # JWT verification
│   ├── 📂 models/
│   │   ├── User.js               # User schema
│   │   └── Message.js            # Message schema
│   ├── 📂 routes/
│   │   ├── authRoutes.js
│   │   └── messageRoutes.js
│   ├── 📂 socket/
│   │   └── socket.js             # Socket.io setup
│   ├── 📄 server.js              # Entry point
│   └── 📄 package.json
├── 📂 frontend/
│   ├── 📂 src/
│   │   ├── 📂 components/
│   │   │   ├── ChatContainer.jsx
│   │   │   ├── MessageInput.jsx
│   │   │   ├── Sidebar.jsx
│   │   │   └── OnlineUsers.jsx
│   │   ├── 📂 pages/
│   │   │   ├── Login.jsx
│   │   │   ├── Signup.jsx
│   │   │   └── Home.jsx
│   │   ├── 📂 store/
│   │   │   ├── useAuthStore.js   # Auth state (Zustand)
│   │   │   └── useChatStore.js   # Chat state (Zustand)
│   │   ├── 📂 utils/
│   │   │   └── axios.js          # API client
│   │   ├── App.jsx
│   │   └── main.jsx
│   └── 📄 package.json
└── 📄 README.md
```

---

## 🚀 Deployment

Deploy your chat app for **FREE** using these platforms:

### Backend (Choose One)

| Platform | Guide |
|----------|-------|
| ![Render](https://img.shields.io/badge/Render-46E3B7?style=flat&logo=render&logoColor=white) | [Deploy to Render](https://render.com/) |
| ![Railway](https://img.shields.io/badge/Railway-0B0D0E?style=flat&logo=railway&logoColor=white) | [Deploy to Railway](https://railway.app/) |

### Frontend (Choose One)

| Platform | Guide |
|----------|-------|
| ![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat&logo=vercel&logoColor=white) | [Deploy to Vercel](https://vercel.com/) |
| ![Netlify](https://img.shields.io/badge/Netlify-00C7B7?style=flat&logo=netlify&logoColor=white) | [Deploy to Netlify](https://netlify.com/) |

### Database

| Platform | Guide |
|----------|-------|
| ![MongoDB Atlas](https://img.shields.io/badge/MongoDB_Atlas-47A248?style=flat&logo=mongodb&logoColor=white) | [Free 512MB Cluster](https://www.mongodb.com/atlas) |

### Quick Deploy Steps

1. **Database** — Create free MongoDB Atlas cluster
2. **Backend** — Deploy to Render/Railway with env variables
3. **Frontend** — Deploy to Vercel/Netlify, set API URL
4. **Done!** — Your chat app is live 🎉

---

## 🔮 Future Scope

| Feature | Description | Priority |
|---------|-------------|----------|
| 👥 **Group Chats** | Create group conversations | High |
| 📷 **Image Sharing** | Send images in chat | High |
| 🔔 **Push Notifications** | Browser notifications for new messages | High |
| ✏️ **Message Editing** | Edit sent messages | Medium |
| 🗑️ **Delete Messages** | Delete messages for everyone | Medium |
| 🎙️ **Voice Messages** | Record and send voice notes | Medium |
| 📹 **Video Calls** | WebRTC video calling | Low |
| 🌙 **Dark/Light Mode** | Theme toggle | Low |
| 😀 **Emoji Picker** | Add emoji support | Low |
| ✅ **Read Receipts** | Message seen indicators | Future |

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. 🍴 Fork the repository
2. 🌿 Create a feature branch (`git checkout -b feature/amazing-feature`)
3. 💾 Commit your changes (`git commit -m 'Add amazing feature'`)
4. 📤 Push to the branch (`git push origin feature/amazing-feature`)
5. 🔃 Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👤 Author

**Armaan Arora**

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/armaan-arora)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/armaan-singh-29bb54247/)

---

## 🙏 Acknowledgements

- [Socket.io](https://socket.io/) — Real-time communication
- [Zustand](https://zustand-demo.pmnd.rs/) — State management
- [DaisyUI](https://daisyui.com/) — Beautiful UI components
- [TailwindCSS](https://tailwindcss.com/) — Utility-first CSS

---

<p align="center">
  ⭐ Star this repo if you found it helpful! ⭐
</p>

<p align="center">
  Made with ❤️ by Armaan Arora
</p>
