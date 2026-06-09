# Smart Study Companion

Smart Study Companion is a premium, full-stack application designed to automatically generate high-quality quizzes on any topic. It features a sleek Light/Dark Mode toggle, detailed study history, and rich visual backgrounds dynamically fetched from Wikipedia.

## Project Structure

- `backend/` - Node.js + Express server handling MongoDB connections, JWT Authentication, and OpenAI integration.
- `frontend/` - React + TypeScript + Vite frontend utilizing TailwindCSS, Framer Motion, and Recharts.

## Prerequisites

- Node.js (v18 or higher recommended)
- MongoDB (running locally or a MongoDB Atlas URI)
- OpenAI API Key

## Setup & Running Locally

### 1. Backend Setup

Open a terminal and navigate to the backend directory:
```bash
cd backend
```

Install dependencies:
```bash
npm install
```

Set up your environment variables by creating a `.env` file (or copying the example):
```bash
cp .env.example .env
```
Open the `.env` file and make sure to set:
- `MONGODB_URI` (e.g., `mongodb://127.0.0.1:27017/smart-study`)
- `OPENAI_API_KEY` (Your OpenAI secret key)
- `JWT_SECRET` (Any long random string)

Start the backend development server:
```bash
npm run dev
```
The server will run on `http://localhost:4000`.

### 2. Frontend Setup

Open a **new** terminal window and navigate to the frontend directory:
```bash
cd frontend
```

Install dependencies:
```bash
npm install
```

Start the frontend Vite development server:
```bash
npm run dev
```

Open your browser and navigate to `http://localhost:5173`. 

## Features

- **Dynamic Quiz Generation**: Choose a topic, difficulty, and question count.
- **Light/Dark Mode**: Premium Slate/Emerald dark mode or clean light mode.
- **Wikipedia Integration**: Automatically fetches contextually relevant background images.
- **Study Analytics**: Track your progress and view past attempts in the History tab.
- **Guest Mode**: Try the app without creating an account.
