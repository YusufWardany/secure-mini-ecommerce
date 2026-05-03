# 🛒 SecureShop

## 📝 About The Project
SecureShop is a mini e-commerce web application built from scratch with a strict "security-first" mindset. The project demonstrates how to build a fully functional online store while implementing multiple layers of defense to protect against the OWASP Top 10 vulnerabilities. 

## 💻 Tech Stack
* Frontend: React.js with Vite
* Backend: Node.js and Express.js
* Database: SQLite
* Security Middleware: Helmet, CORS, csurf, express-rate-limit
* Authentication: JWT and bcrypt

## 🔒 Security Implementations
* Server-side input validation and sanitization using express-validator.
* Complete prevention of SQL Injection using parameterized queries for all database interactions.
* Cross-Site Scripting (XSS) mitigation via DOMPurify on the client and Helmet HTTP headers on the server.
* CSRF tokens required and validated for all state-changing requests (POST, PUT, DELETE).
* Secure session management with JWTs stored exclusively in HttpOnly cookies.
* Brute-force protection using rate limiting and a 15-minute account lockout after 5 failed login attempts.
* Strict Role-Based Access Control (RBAC) preventing unauthorized privilege escalation.

## 🚀 Application Features
* Product catalog with search, filtering, and pagination functionalities.
* Secure multi-step checkout process and shopping cart validation.
* Dedicated Admin dashboard with sales analytics, inventory management, and charts.
* Staff portal for tracking, updating, and delivering customer orders.
* Responsive design with an integrated Dark/Light mode toggle.

## 🛠️ Installation & Setup

1. Clone the repository to your local machine.
2. Open a terminal, navigate to the `backend` folder, and run `npm install`.
3. Start the backend server by running `node server.js` (this automatically seeds the database with Admin and Staff accounts).
4. Open a new terminal, navigate to the `frontend` folder, and run `npm install`.
5. Start the frontend development server by running `npm run dev`.
6. Open your browser and navigate to `http://localhost:5173`.

## 👥 Contributors
* Youssif Yasser Wardany
* Hazem Khaled Kassem
* Omar Islam
