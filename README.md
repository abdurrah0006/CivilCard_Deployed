# Civil Card — Avengers Card Store

A full-stack superhero trading-card storefront. The **HTML, CSS, and JavaScript frontend** connects to an **Express and MongoDB backend** for product listings, account access, cart checkout, and order history.

## Features

- Browse a product collection and open product details
- Search products and filter by team
- Add products to a browser-persisted cart
- Register and sign in with token-based authentication
- Submit orders and view order history
- Responsive storefront pages for home, collections, product details, cart, account, and orders

## Tech stack

- HTML, CSS, and vanilla JavaScript
- Node.js and Express
- MongoDB with Mongoose
- JWT authentication and bcrypt password hashing

## Run locally

Install and start the backend:

```bash
cd backend
npm install
npm run dev
```

Create `backend/.env` with:

```env
PORT=5000
MONGO_URI=<your-mongodb-connection-string>
JWT_SECRET=<your-random-secret>
```

Serve the `frontend/` directory with a local static web server, then open `frontend/index.html` through that server. The frontend currently points to the deployed API URL in its JavaScript files; change the API base URL to your local backend when developing locally.

## Project structure

- `frontend/` — storefront pages, styles, scripts, and product data
- `backend/` — Express server, authentication, product and order routes, and database models
- `backend/defaults/` — default card artwork

Use your own database and credentials for local development. Do not commit `.env` files.
