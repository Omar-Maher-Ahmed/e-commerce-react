# 🛍️ E-Commerce Frontend

Frontend for a modular e-commerce REST API built with Node.js, Express, and MongoDB. This frontend consumes the backend APIs and provides a full shopping experience.

---

## 📦 Tech Stack

- React.js
- React Router DOM
- Axios
- Tailwind CSS / Bootstrap
- React Hook Form + Yup (Validation)
- JWT Authentication
- Context API / Redux Toolkit

---

## 📁 Folder Structure

src/
├── components/ # Reusable components
├── pages/ # Page-level components (routes)
├── services/ # API logic (axios calls)
├── context/ # Auth & Global state
├── utils/ # Helpers, formatters, etc
├── App.jsx # App Router
└── main.jsx # Entry point


---

## 🔐 Authentication

- JWT token saved in localStorage
- Sent in every secured API call in `Authorization` header
- Protected routes implemented using a `ProtectedRoute` component

---

## 🧭 Routes

| Route             | Description |
|------------------|-------------|
| `/`              | Landing page |
| `/register`      | Register new user |
| `/login`         | Login with email/password |
| `/products`      | View all products |
| `/product/:id`   | Product details |
| `/cart`          | View & manage cart |
| `/checkout`      | Place an order |
| `/orders`        | View user orders |

---

## 🧰 Setup Instructions

```bash
# 1. Clone the repository
git clone https://github.com/your-username/ecommerce-frontend.git
cd ecommerce-frontend

# 2. Install dependencies
npm install

# 3. Run the development server
npm run dev

# 4. Set your API base URL in .env file
VITE_API_URL=http://localhost:5000/api
