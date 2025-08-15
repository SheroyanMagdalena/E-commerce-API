# E-commerce API

A RESTful API built with **Node.js**, **Express**, and **MongoDB (Mongoose)** for managing users, products, carts, and orders in an e-commerce platform.

## ✨ Features
- **User Management** — Register, login, authentication (JWT), profile
- **Product Management** — CRUD operations for products
- **Cart Management** — Add/remove items, view cart
- **Order Management** — Place orders, view history
- **MongoDB Integration** — Data persistence via Mongoose
- **Environment Config** — Secure config using `dotenv`
- **Middleware** — Authentication and error handling

## 🧱 Tech Stack
- **Runtime**: Node.js
- **Framework**: Express
- **Database**: MongoDB + Mongoose
- **Environment**: dotenv
- **Other**: JWT for authentication

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone <your-repo-url>.git
cd E-commerce-API-main
```

### 2. Install dependencies
```bash
npm install
```

### 3. Environment variables
Create a `.env` file in the project root:
```env
PORT=5000
MONGO_URI=mongodb://localhost:27017/ecommerce
JWT_SECRET=your_jwt_secret
```

### 4. Run the server
```bash
npm start
```
or for development:
```bash
npm run dev
```

## 📂 API Routes

| Resource  | Method | Endpoint              | Description |
|-----------|--------|-----------------------|-------------|
| Users     | POST   | `/api/users/register` | Register new user |
|           | POST   | `/api/users/login`    | Login user |
| Products  | GET    | `/api/products`       | List products |
|           | POST   | `/api/products`       | Create product |
| Carts     | GET    | `/api/carts`          | Get user cart |
|           | POST   | `/api/carts`          | Add to cart |
| Orders    | GET    | `/api/orders`         | List orders |
|           | POST   | `/api/orders`         | Create order |

> Actual endpoints may vary based on your implementation.

## 🛠 Project Structure
```
E-commerce-API-main/
├── config/           # DB and environment configuration
├── controllers/      # Route handlers
├── middlewares/      # Auth, error handling
├── models/           # Mongoose schemas
├── routes/           # API routes
├── utils/            # Helper functions
├── server.js         # App entry point
└── package.json
```



