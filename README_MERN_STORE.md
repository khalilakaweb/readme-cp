# MERN Store — Draft Repository (README)

## Project name
**mern-store**  
(or `tunis-mern-store`, `interact-mern-store` — pick whichever you prefer)

---

## Short description
A full-stack e-commerce store built with the MERN stack (MongoDB, Express, React, Node) that demonstrates user authentication, product management, shopping cart, and checkout flow. The app highlights responsive UI, RESTful APIs, and database modeling with Mongoose. Implemented with TypeScript where appropriate.

---

## Goals / Learning objectives
- Build a production-style full-stack web application end-to-end.  
- Practice React (and Next.js routing / SSR where desired) for front-end UI.  
- Design and consume REST APIs with Node.js + Express.  
- Model data and interact with MongoDB using Mongoose.  
- Add authentication/authorization (JWT or session).  
- Implement responsive layout (HTML, CSS, optionally Tailwind or plain CSS).  
- Use TypeScript in front-end and/or back-end for type safety.  
- Deploy a demo (optional for later phases) and demonstrate CI-friendly repo structure.  

---

## Core features (minimum viable product for Lab Phase)
1. Product listing (CRUD for admin)  
2. Product detail page  
3. Shopping cart (add/remove, quantity)  
4. User signup / login (JWT)  
5. Checkout page (no real payments required — simulate)  
6. REST API endpoints for products, users, orders  
7. Database schemas with Mongoose  
8. Simple responsive UI (mobile + desktop)  

---

## Stretch features (after MVP)
- Product search & filters  
- User profile & order history  
- Admin dashboard with analytics  
- File uploads for product images (Cloudinary or local)  
- Next.js SSR/SSG for product pages  
- Payment integration mock (Stripe test mode)  
- Tests (Jest + React Testing Library / supertest)  

---

## Tech stack
- **Front-end:** React (create-react-app or Next.js), TypeScript (optional), HTML, CSS  
- **Back-end:** Node.js, Express.js, TypeScript (optional)  
- **Database:** MongoDB, Mongoose  
- **Auth:** JWT  
- **Dev tools:** Git, ESLint, Prettier, dotenv  
- **Optional:** Tailwind CSS or plain CSS modules  

---

## Repository structure (suggested)
```
/mern-store
├─ /client            
│  ├─ package.json
│  ├─ src/
│  │  ├─ components/
│  │  ├─ pages/ (if Next.js)
│  │  └─ styles/
├─ /server
│  ├─ package.json
│  ├─ src/
│  │  ├─ controllers/
│  │  ├─ models/
│  │  ├─ routes/
│  │  └─ app.ts (or app.js)
├─ .env.example
├─ README.md
└─ .gitignore
```

---

## How to run (local development)
1. Clone repo:  
```bash
git clone https://github.com/<your-username>/mern-store.git
cd mern-store
```

2. Create `.env` files (see `.env.example`) for server (MONGO_URI, JWT_SECRET) and client (API_URL).  
3. Start server:  
```bash
cd server
npm install
npm run dev
```

4. Start client:  
```bash
cd ../client
npm install
npm run dev
```

5. Open [http://localhost:3000](http://localhost:3000) (client) and the server API runs at [http://localhost:5000](http://localhost:5000).  

---

## Lab Phase submission (what to include)
- Create the draft repository with the exact repo name (e.g., `mern-store`).  
- Include this `README.md` in the repo root.  
- Add basic code scaffolding:  
  - Server: an `app.js`/`app.ts` with Express, a sample `/api/products` route returning JSON.  
  - Client: a simple React page showing a product list fetched from `/api/products`.  
- Add `.env.example` with placeholders.  
- Commit and push; submit repository link as your Lab Phase draft.  

---

## Milestones / Suggested schedule (for the Lab Phase)
- **Day 1–2:** Repo scaffold (client + server), basic API route, connect to MongoDB (or mock).  
- **Day 3–5:** Products model + CRUD endpoints; simple front-end listing.  
- **Day 6–8:** Authentication (signup/login) and shopping cart UI.  
- **Day 9–11:** Checkout flow + order endpoints.  
- **Day 12–14:** Polishing, responsiveness, README, prepare instructor demo.  

---

## Roles & instructor assistance
- **If partnered:** Agree on the project choice, split tasks (front-end / back-end / DB / deployment). Instructor will review your plan and help align scope.  
- **If solo:** Instructor will help you choose features and adjust scope. Request code reviews or help with tricky bugs.  
- Instructor checks for: repo name, README, at least one working API endpoint, and a simple client page fetching that endpoint.  

---

## Initial issues (create these in GitHub for Lab Phase)
1. Scaffold server and client (create initial branches).  
2. Implement `GET /api/products` returning sample data.  
3. Create React page to fetch and display products.  
4. Add `.env.example` and README (this file).  
5. Connect MongoDB and create Product model.  

---

## Notes for the instructor
This draft repo demonstrates an MVP for a MERN e-commerce store. For the Lab Phase we’ll present a working API endpoint and a client page to fetch it. Requesting support for MongoDB connection setup, authentication flow, and deployment guidance.  

---

## Contact / Contributors
- **Author:** Mohamed Khalil Bibi  
- **Role:** Full stack developer (Bootcamp)  
- **Contact:** [Add your email or bootcamp handle here]  
