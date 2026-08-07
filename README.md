# Cohort 9 — MERN Assignment

## Notes Manager

A full-stack Notes Manager application developed as part of the **Cohort 9 MERN (Node.js + React.js) assignment**.

The application allows users to create an account, log in securely, and manage their personal notes through a React frontend and Node.js/Express backend.

---

## Tech Stack

### Frontend

- React.js
- React Router
- Axios
- CSS
- Vite

### Backend

- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT Authentication
- bcrypt

### Development Tools

- Git
- GitHub
- Postman
- VS Code

---

## Project Structure

```text
cohort-9-mern-16209-syed/
│
├── frontend/
│   ├── src/
│   │   ├── api/
│   │   ├── components/
│   │   ├── pages/
│   │   └── ...
│   ├── package.json
│   └── ...
│
├── backend/
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── utils/
│   ├── .gitignore
│   ├── package.json
│   └── server.js
│
└── README.md
```

---

## Quick Start

### 1. Backend

Open a terminal and run:

```bash
cd backend
npm install
npm run dev
```

The backend server will start using the development script configured in `package.json`.

### 2. Frontend

Open another terminal and run:

```bash
cd frontend
npm install
npm run dev
```

The frontend will start using Vite.

---

## Environment Variables

Create a `.env` file inside the `backend` folder.

Example:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
```

Do not commit `.env` to GitHub.

---

## Features

- User registration
- User login
- JWT authentication
- Protected routes
- Create notes
- View notes
- Search notes
- Edit notes
- Delete notes
- User profile
- Logout

---

## API

### Authentication

| Method | Endpoint | Description |
|---|---|---|
| POST | `/auth/register` | Register a new user |
| POST | `/auth/login` | Login user |

### Notes

| Method | Endpoint | Description |
|---|---|---|
| GET | `/notes` | Get user notes |
| POST | `/notes` | Create a note |
| GET | `/notes/:id` | Get a specific note |
| PUT | `/notes/:id` | Update a note |
| DELETE | `/notes/:id` | Delete a note |

> Make sure these endpoints match your actual `authRoutes.js` and `notesRoutes.js`.

---

## Security

The application uses:

- bcrypt for password hashing
- JWT for authentication
- Protected routes
- Environment variables for sensitive configuration
- `.gitignore` to exclude `.env` and `node_modules`

---

## Git Workflow

The project uses feature branches for development.

Example:

```text
feature/backend/controllers
feature/backend/middleware
feature/backend/routes
feature/backend/services
feature/frontend/components
```

Changes are committed and submitted through GitHub Pull Requests.

---

## Author

**Syed Mustafa Hussain**

**Cohort 9 — MERN Assignment**
