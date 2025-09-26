# term-insurance-chatbot

The Chatbot helps users discover and compare term insurance plans available in the market. This repository contains a small FastAPI backend and a Next.js frontend scaffold to demonstrate a conversational UI for insurance guidance.

## Executive Summary

A lightweight chatbot prototype that provides information about term insurance plans. The project is split into two main components: a FastAPI backend that serves APIs and a Next.js frontend built with React for the user interface.

## Architecture Overview

- System Architecture: The app uses a client-server architecture. The Next.js frontend communicates with the FastAPI backend over HTTP (REST). The backend exposes API endpoints (currently a root health endpoint) and is intended to host the chatbot logic or proxy to an LLM or knowledge service.
- Technology Stack: FastAPI (backend), Uvicorn (ASGI server), Python for backend; Next.js, React, and Tailwind CSS for frontend.
- Component Interaction: Frontend calls backend endpoints (e.g., /api/chat or root /) to send user messages and receive responses. Static assets are served by Next.js in production.
- Deployment Architecture: Each component can be deployed independently. Common choices: Vercel for frontend, and a containerized FastAPI app on platforms like AWS ECS, Azure App Service, or Render. Use environment variables for runtime configuration.

## Project Structure

- `backend/` - FastAPI application, requirements and backend docs
- `frontend/` - Next.js application, scripts, and frontend docs
- `.github/prompts/` - Documentation prompt templates and guidance
- `README.md` - This top-level project overview

## Getting Started

Prerequisites: Python 3.11+, Node.js 18+ (or current LTS), and npm/yarn.

Backend (quick start):

1. cd into `backend`
2. Create a virtual environment and install dependencies: `python -m venv .venv; .\.venv\Scripts\Activate.ps1; pip install -r requirements.txt`
3. Run the app for development: `uvicorn main:app --reload --port 8000`

Frontend (quick start):

1. cd into `frontend`
2. Install dependencies: `npm install`
3. Start development server: `npm run dev`

## Change History

### 2025-09-27 - v0.1 - FEATURE

**Components Affected**: README, backend docs, frontend docs
**Summary**: Added structured documentation for project, backend, and frontend following repository documentation guidelines.
**Details**:

- Created high-level architecture overview and technology stack.
- Added getting started steps and basic run instructions for backend and frontend.
- Recorded this changelog entry.
  **Breaking Changes**: None
  **Migration Notes**: None

---

## Contributing

If you'd like to contribute, open an issue or a pull request describing the change. For documentation updates, follow the template in `.github/prompts/update_readme.md`.
