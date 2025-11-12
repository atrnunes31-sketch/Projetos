GlowUp365 - Web Starter Project

This package contains a minimal web-ready starter for GlowUp365:
- backend/ : Express.js backend (API stubs)
- frontend/react/ : Minimal React app (entry point & pages)
- landing.html : Static landing page template
- openapi.yaml : Basic API spec
- onboarding.json : Questionnaire + rules
- schema.sql : Basic SQL schema

How to run locally (development):
1) Backend
   cd backend
   npm install
   npm start
   Backend runs on http://localhost:3000

2) Frontend (React)
   cd frontend/react
   npm install
   npm start
   Frontend runs on http://localhost:3001 (or 3000—if port conflict, change)

Notes:
- This is starter code. Replace secrets and add production-ready configs before deploying.
- For payments, configure STRIPE_SECRET and MercadoPago credentials.


## Added by assistant
- Dockerfile for backend and frontend
- docker-compose.yml to run backend, frontend and postgres
- docs/stripe.md and docs/mercadopago.md with integration notes
- expanded React frontend with Onboarding, Dashboard, Plans
- GitHub Actions CI workflow (basic)

## Quick deploy (local)
1. Copy .env values, set STRIPE_SECRET and STRIPE_WEBHOOK_SECRET
2. docker-compose up --build
3. Access frontend at http://localhost:3001 and backend at http://localhost:3000
