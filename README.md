## Petal Boutique

Luxury 3D-enabled boutique e-commerce experience with selective WebGL, role-based auth, analytics-driven trending/best-sellers, and employee inventory ops.

### Payments
- **Cash on Delivery (COD)** is supported/communicated in the UI (MVP payment method).

### Tech
- **Frontend**: React (Vite) + Tailwind CSS + React Three Fiber (selective 3D)
- **Backend**: Node.js + Express + JWT auth (Customer/Employee roles)
- **DB**: MongoDB (Mongoose)

### Monorepo layout
- `apps/web`: React app
- `apps/api`: Express API

### Quickstart (local)
Prereqs: Node 18+ and MongoDB running (or a MongoDB Atlas URI).

1) Create env files
- `apps/api/.env`:
  - `PORT=4000`
  - `MONGODB_URI=mongodb://127.0.0.1:27017/petal_boutique`
  - `JWT_ACCESS_SECRET=change_me_access_secret`
  - `JWT_REFRESH_SECRET=change_me_refresh_secret`
  - `CORS_ORIGIN=http://localhost:5173`
  - `STRIPE_SECRET_KEY=` (optional)
  - `CLOUDINARY_URL=` (optional)

- `apps/web/.env`:
  - `VITE_API_URL=http://localhost:4000`

2) Install deps (from repo root)
```bash
npm install
```

3) Run
```bash
npm run dev
```

### Branding requirement
The footer intentionally displays: **A Developed Product by Blaze**

