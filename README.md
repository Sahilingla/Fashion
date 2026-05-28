# Fashion 

A full-stack e-commerce web application for buying and selling clothes — featuring a customer-facing storefront, 
a REST API backend, and an admin dashboard for managing products and orders.

🚀 Live Demo

Deployed Link :- https://heroic-bonbon-d3b3d8.netlify.app/

---

## 🗂️ Project Structure

```
Fashion/
├── frontend/      # React customer storefront
├── backend/       # Node.js + Express REST API
└── admin/         # Admin dashboard (product & order management)
```

---

##  Features

### Customer (Frontend)
- Browse and search clothing products
- Product detail pages with images and sizing
- Add to cart and checkout flow
- User registration and login (JWT authentication)

### Admin Dashboard
- Add, edit, and delete products
- View and manage orders
- Upload product images

### Backend API
- RESTful API built with Node.js & Express
- JWT-based authentication and authorization
- MongoDB database with Mongoose ODM
- Secure password hashing with bcryptjs

---

## 🛠️ Tech Stack

| Layer     | Technology                     |
|-----------|------------------------------- |
| Frontend  | React.js,Axios,React Router    |
| Backend   | Node.js, Express.js            |
| Database  | MongoDB                        |
| Auth      | JSON Web Tokens (JWT), bcryptjs|

---




### 2. Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file in the `/backend` directory:

```env
PORT=4000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
```

Start the backend server:

```bash
npm run dev
```

The API will run on `http://localhost:4000`

---

### 3. Frontend Setup

```bash
cd ../frontend
npm install
npm run dev
```

The frontend will run on `http://localhost:5173`

---

### 4. Admin Setup

```bash
cd ../admin
npm install
npm run dev
```

The admin panel will run on `http://localhost:5174`

---

## 📡 API Overview

| Method | Endpoint              | Description              |
|--------|-----------------------|--------------------------|
| POST   | `/api/user/register`  | Register a new user      |
| POST   | `/api/user/login`     | Login and get JWT token  |
| GET    | `/api/product/list`   | Get all products         |
| POST   | `/api/product/add`    | Add a product (admin)    |
| DELETE | `/api/product/remove` | Remove a product (admin) |
| POST   | `/api/order/place`    | Place an order           |
| GET    | `/api/order/list`     | Get all orders (admin)   |

---

## 🔐 Environment Variables

| Variable    | Description                        |
|-------------|-----------------------------------|
| `PORT`      | Port the backend runs on           |
| `MONGO_URI` | MongoDB connection string          |
| `JWT_SECRET`| Secret key for signing JWT tokens  |

---

## 📁 Folder Details

### `/backend`
- `server.js` — Entry point, Express app setup
- `/routes` — API route definitions
- `/controllers` — Business logic
- `/models` — Mongoose schemas (User, Product, Order)
- `/middleware` — Auth middleware (JWT verification)

### `/frontend`
- `/src/pages` — Page components (Home, Product, Cart, Login)
- `/src/components` — Reusable UI components
- `/src/context` — React Context for cart and auth state

### `/admin`
- Dashboard for adding/removing products and managing orders

---

  
