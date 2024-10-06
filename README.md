
# GadgetHub

**GadgetHub** is a full-stack e-commerce platform that allows users to browse products, add them to a cart, and make purchases. The platform includes user authentication, secure payment integration using Stripe, and an easy-to-use product management system for administrators.

## Table of Contents
- [Project Overview](#project-overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Screenshots](#screenshots)
- [Contributors](#contributors)
- [License](#license)

## Project Overview

GadgetHub is built to provide a seamless shopping experience for users and a convenient management system for admins. Users can browse through various electronic gadgets, view product details, and securely purchase them. The platform includes payment integration via Stripe and ensures user authentication to protect data and transactions.

## Features

- User Registration and Login (with JWT Authentication)
- Browse Products by Category
- Add to Cart and Checkout
- Secure Payment Gateway (Powered by Stripe)
- Admin Panel to Add/Update Products
- Responsive Design for Mobile and Desktop

## Technologies Used

- **Frontend:**
  - React.js
  - Tailwind CSS
  - Axios
  - React Icons
- **Backend:**
  - Node.js
  - Express.js
  - MongoDB (Mongoose ORM)
- **Payment Integration:**
  - Stripe API
- **Deployment:**
  - Vercel (Frontend)
  - Heroku (Backend)

## Installation

### Prerequisites
- Node.js (version >= 14)
- MongoDB (Ensure MongoDB is running locally or provide a connection string)
- Stripe Account (for payment integration)

### Steps to Set Up Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/GadgetHub.git
   ```

2. Navigate to the backend directory and install dependencies:
   ```bash
   cd backend
   npm install
   ```

3. Set up environment variables by creating a `.env` file in the backend folder with the following:
   ```bash
   MONGO_URI=your_mongodb_connection_string
   STRIPE_SECRET_KEY=your_stripe_secret_key
   JWT_SECRET=your_jwt_secret
   FRONTEND_URL=http://localhost:3000
   ```

4. Start the backend server:
   ```bash
   npm start
   ```

5. In a new terminal window, navigate to the frontend directory and install dependencies:
   ```bash
   cd frontend
   npm install
   ```

6. Start the frontend:
   ```bash
   npm start
   ```

7. Open your browser and navigate to `http://localhost:3000`.

## Usage

1. Users can register or log in to their accounts.
2. Browse through the available gadgets on the homepage.
3. Add products to the cart and proceed to checkout.
4. Make payments using the integrated Stripe payment gateway.

### Admin Panel

- Navigate to `/admin` (accessible only by authorized admin users).
- Manage products, including adding, updating, or removing items from the store.

## API Endpoints

- **User Authentication**
  - `POST /api/register`: Create a new user account
  - `POST /api/login`: Log in with existing credentials
- **Product Management**
  - `GET /api/products`: Fetch all products
  - `POST /api/products`: Add a new product (admin only)
  - `PUT /api/products/:id`: Update product details (admin only)
  - `DELETE /api/products/:id`: Delete a product (admin only)
- **Cart and Checkout**
  - `POST /api/cart`: Add items to the cart
  - `POST /api/checkout`: Process payment using Stripe

## Contributors

- **Mohd. Azam Siddique** - Full Stack Developer
