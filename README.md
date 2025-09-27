HealthBridge AI
============================================
This scaffold contains a minimal AI-enabled telemedicine MVP:
- Frontend: React + Vite + Tailwind (pages: Dashboard, SymptomChecker, FirstAid, FindCare, Profile)
- Backend: Express + Multer + example /api/analyze route that accepts text or audio and returns AI analysis (requires configuring an LLM provider)
- services/llm.js: wrapper functions to call OpenAI or Hugging Face (stubs and examples included)
- .env.sample files for both frontend and backend

Important:
- This project is a starting point. To enable real AI functionality, add your API keys to backend/.env and choose the provider (OpenAI or Hugging Face).
- See backend/README_AI.md for setup details for AI providers.

To run locally:
1. Start MongoDB (optional for providers list) or use Docker.
2. Configure backend/.env (copy from .env.sample).
3. Install and run backend:
   cd backend
   npm install
   node server.js
4. Install and run frontend:
   cd frontend
   npm install
   npm run dev
5. Open http://localhost:5173

