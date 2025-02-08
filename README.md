# Full-Stack React + FastAPI Application

This is a modern full-stack application built with React, TypeScript, and FastAPI.

## Project Structure

```
.
├── backend/                 # FastAPI backend
│   ├── Dockerfile          # Backend container configuration
│   ├── main.py            # Main FastAPI application
│   └── requirements.txt    # Python dependencies
├── src/                    # React frontend source
│   ├── App.tsx            # Main React component
│   ├── main.tsx           # React entry point
│   └── index.css          # Global styles
├── docker-compose.yml      # Docker compose configuration
├── Dockerfile             # Frontend container configuration
└── package.json           # Node.js dependencies
```

## Getting Started

1. Clone the repository
2. Install dependencies:
   ```bash
   npm install        # Frontend dependencies
   cd backend
   pip install -r requirements.txt  # Backend dependencies
   ```

3. Run with Docker:
   ```bash
   docker-compose up --build
   ```

   Or run separately:
   ```bash
   # Frontend
   npm run dev

   # Backend
   cd backend
   uvicorn main:app --reload
   ```

## Development

- Frontend runs on http://localhost:3000
- Backend API runs on http://localhost:8000
- API documentation available at http://localhost:8000/docs

## Technologies Used

- Frontend:
  - React
  - TypeScript
  - Tailwind CSS
  - Vite
  - Lucide React (icons)

- Backend:
  - FastAPI
  - Python 3.11
  - Uvicorn

- Infrastructure:
  - Docker
  - Docker Compose
  - Nginx (production)