# MERN Backend Auth Starter

Skip repetitive backend setup and start building your MERN applications faster.

This repository was originally created for my own projects because I found myself rewriting the same backend setup every time I started a new MERN application — MongoDB connection, JWT authentication, refresh tokens, protected routes, error handling, folder structure, environment configuration, and other boilerplate.

Instead of rebuilding everything from scratch for every project, I decided to create a reusable starter template that provides a production-ready backend foundation.

If you're building a MERN application and don't want to spend time setting up authentication and backend architecture again, feel free to use this starter.

## Features

* JWT Authentication
* Refresh Token Rotation
* Protected Routes
* Password Hashing with bcrypt
* MongoDB & Mongoose Integration
* Cookie-based Authentication
* Environment Variable Configuration
* Global Error Handling Utilities
* Standardized API Responses
* Scalable Folder Structure
* Prettier Configuration

## Project Structure

```text
backend/
├── src/
│   ├── controllers/
│   ├── db/
│   ├── middlewares/
│   ├── models/
│   ├── routes/
│   ├── utils/
│   ├── app.js
│   ├── constants.js
│   └── index.js
├── .env.sample
├── .gitignore
├── .prettierignore
├── .prettierrc
├── package.json
└── package-lock.json
```

## Getting Started

### Clone the Repository

```bash
git clone https://github.com/betterversionofpuja/mern-backend-auth-starter.git
```

### Install Dependencies

```bash
cd mern-backend-auth-starter/backend
npm install
```

### Create Environment Variables

Create a `.env` file using `.env.sample` as reference.

```env
PORT=8000

NODE_ENV=development

CORS_ORIGIN=*

MONGODB_URI=

ACCESS_TOKEN_SECRET=
ACCESS_TOKEN_EXPIRY=1d

REFRESH_TOKEN_SECRET=
REFRESH_TOKEN_EXPIRY=10d
```

### Run the Server

```bash
npm run dev
```

Server will start on:

```text
http://localhost:8000
```

## Available Endpoints

### Authentication

```http
POST /api/v1/users/register
POST /api/v1/users/login
POST /api/v1/users/logout
POST /api/v1/users/refresh-token
```

### User

```http
GET  /api/v1/users/profile
PUT  /api/v1/users/profile
POST /api/v1/users/change-password
```

## Typical Usage

1. Clone the repository.
2. Configure MongoDB and environment variables.
3. Start the backend server.
4. Create your frontend application (React, Next.js, etc.).
5. Focus on building product features instead of backend boilerplate.

## Why This Exists

I built this starter primarily for my own MERN projects. Over time I realized other developers repeatedly face the same problem of setting up authentication and backend architecture from scratch.

This repository aims to provide a clean starting point so developers can spend less time on setup and more time building.

## License

MIT License

## Author

Puja Kumari

GitHub: https://github.com/betterversionofpuja
