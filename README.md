
# 🎵 Music Platform

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![React](https://img.shields.io/badge/frontend-React-61DAFB.svg?style=flat-square&logo=react&logoColor=black)
![Node](https://img.shields.io/badge/backend-Node.js-339933.svg?style=flat-square&logo=node.js&logoColor=white)
![MongoDB](https://img.shields.io/badge/database-MongoDB-47A248.svg?style=flat-square&logo=mongodb&logoColor=white)
![Tailwind](https://img.shields.io/badge/styling-Tailwind_CSS-38B2AC.svg?style=flat-square&logo=tailwind-css&logoColor=white)

A full-stack social music and audiobook platform enabling users to upload, stream, and share audio content, manage friends, and interact in real time. Built with the MERN stack (MongoDB, Express, React, Node.js) and powered by **Socket.IO** for real-time features and **Cloudinary** for media management.

---

## ✨ Features

*   **🎧 seamless Streaming**: High-quality audio streaming using **Howler.js**.
*   **📂 Cloud Storage**: Secure upload and storage for songs and audiobooks via **Cloudinary**.
*   **👥 Social Connectivity**: 
    *   Search and add friends.
    *   Real-time friend requests (Accept/Decline).
    *   View friend activity and status.
*   **💬 Real-Time Interaction**: 
    *   **Socket.IO** integration for instant messaging.
    *   Live notifications for friend requests and messages.
    *   Real-time presence (Online/Offline status).
*   **🔐 Secure Authentication**: JWT-based authentication using **Passport.js**.
*   **🎨 Modern UI/UX**: Responsive and sleek design built with **React** and **Tailwind CSS**.

---

## 🛠️ Tech Stack

### Frontend
*   **React** (v18) - Component-based UI.
*   **Tailwind CSS** - Utility-first styling.
*   **Socket.io-client** - Real-time client communication.
*   **Howler.js** - Audio playback control.
*   **Axios** - HTTP client.
*   **Craco** - Create React App Configuration Override.

### Backend
*   **Node.js & Express** - Server-side logic and REST API.
*   **MongoDB & Mongoose** - NoSQL database and odm.
*   **Socket.io** - Real-time bidirectional event-based communication.
*   **Passport.js** (JWT) - Authentication middleware.
*   **Cloudinary** - Cloud media management.
*   **Bcrypt** - Password hashing.

---

## 🚀 Getting Started

Follow these instructions to set up the project locally.

### Prerequisites
*   [Node.js](https://nodejs.org/) (v14+)
*   [MongoDB](https://www.mongodb.com/) (Local or Atlas)
*   [Cloudinary Account](https://cloudinary.com/)

### Installation

#### 1. Clone the Repository
```bash
git clone https://github.com/SoumyadityaDutta-rgb/Victor-Music-Streaming-Platform
cd Music-Platform-main
```

#### 2. Backend Setup
Navigate to the backend directory and install dependencies:
```bash
cd spotify_backend
npm install
```

Create a `.env` file in the `spotify_backend` directory with the following variables:
```env
PORT=3000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
```

Start the backend server:
```bash
npm start
# OR for development with nodemon
npm run dev
```

#### 3. Frontend Setup
Navigate to the frontend directory and install dependencies:
```bash
cd ../my-app
npm install
```

Start the React development server:
```bash
npm start
```
The application should now be running on `http://localhost:8000` (or the port specified in your frontend config).

---

## 📂 Project Structure

```bash
Music-Platform-main/
├── my-app/                 # ⚛️ React Frontend
│   ├── public/
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── utils/          # Helper functions
│   │   ├── App.js          # Main Application component
│   │   └── ...
│   ├── tailwind.config.js
│   └── package.json
│
└── spotify_backend/        # 🔙 Node/Express Backend
    ├── models/             # Mongoose Schemas (User, Song, etc.)
    ├── routes/             # API Routes
    ├── utils/              # Helper utilities
    ├── index.js            # Server entry point
    ├── socketManager.js    # Socket.IO logic
    └── package.json
```

---

## 🔌 API Endpoints

### Authentication
| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `POST` | `/auth/signup` | Register a new user |
| `POST` | `/auth/login` | Login user and return JWT |

### Friends & Social
| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `GET` | `/friends/search/:query` | Search for users |
| `POST` | `/friends/request` | Send a friend request |
| `GET` | `/friends/list` | Get list of friends |
| `POST` | `/friends/recommend` | Recommend a song |

### Real-Time Events (Socket.IO)
*   `connection`: Client connects
*   `privateMessage`: Send a private message
*   `friendOnline`: Notify friends when user comes online
*   `friendOffline`: Notify friends when user goes offline
*   `messageSent`: Confirmation of message sent

---

## 🤝 Contribution

Contributions are welcome! Please follow these steps:
1.  **Fork** the repository.
2.  Create a new **Branch** (`git checkout -b feature/AmazingFeature`).
3.  **Commit** your changes (`git commit -m 'Add some AmazingFeature'`).
4.  **Push** to the branch (`git push origin feature/AmazingFeature`).
5.  Open a **Pull Request**.

---

## 📝 License

Distributed under the MIT License. See `LICENSE` for more information.

---

## 📞 Contact

**Soumyaditya Dutta** - [soumyadityadutta40@gmail.com](mailto:soumyadityadutta40@gmail.com)

