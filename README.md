# Quick-AI

Quick-AI is a web-based AI SaaS project built as a full-stack college project using the PERN stack (PostgreSQL, Express, React, and Node.js).

## Project Overview

The project explores how AI-powered features can be exposed through a modern web application with a separate frontend and backend. It is intended as a practical full-stack project for learning authentication, API integration, database-backed applications, and AI workflows.

## Tech Stack

- **Frontend:** React 19, Vite, JavaScript
- **Backend:** Node.js, Express 5
- **Database:** PostgreSQL
- **Authentication:** Clerk
- **AI integrations:** OpenAI and Groq SDKs
- **Media:** Cloudinary
- **Architecture:** REST API + client application
- **Deployment:** Vercel frontend deployment

## Repository layout

```text
Quick-AI-/
├── client/     # React + Vite frontend
├── server/     # Express API and integrations
└── README.md
```

## Getting Started

### Prerequisites

- Node.js 18+ (Node.js 20+ recommended)
- A PostgreSQL database
- Clerk credentials for authentication
- API credentials for the AI/media services used by the features you enable

### 1. Install frontend dependencies

```bash
cd client
npm install
```

Start the frontend in development mode:

```bash
npm run dev
```

The client package also provides `npm run lint`, `npm run build`, and `npm run preview` for validation and production-preview workflows.

### 2. Install backend dependencies

From the repository root:

```bash
cd server
npm install
```

Start the API with automatic restart during development:

```bash
npm run server
```

For a production-style start:

```bash
npm start
```

The Express server listens on `PORT` when provided, otherwise it defaults to `3000`.

### Environment variables

The backend loads configuration through `dotenv`. Keep API keys, database credentials, authentication secrets, and other private configuration in environment variables. Do not commit `.env` files or production credentials to Git.

Because the exact credentials and feature configuration depend on the enabled integrations, check the imports under `server/configs/` and the route implementations under `server/routes/` before creating your local environment file.

## Deployment

The frontend has been deployed at:

**https://client-seven-dusky-39.vercel.app**

For a complete deployment, configure the same authentication, database, AI, and Cloudinary environment values in the hosting provider rather than committing them to the repository.

## What I Learned

This project demonstrates practical experience with:

- Building a React-based web interface.
- Connecting a frontend to an Express/Node.js backend.
- Working with PostgreSQL-backed application data.
- Designing API-driven application flows.
- Integrating AI functionality into a full-stack application.
- Preparing a JavaScript application for deployment.

## Future Improvements

- Add automated frontend/backend tests.
- Add CI validation for pull requests.
- Improve API error handling and user-facing loading states.
- Add stronger request validation and rate limiting for production use.
- Document individual AI features and API endpoints as they evolve.

## Author

**Amit Yadav** — [GitHub](https://github.com/Hisokak49)
