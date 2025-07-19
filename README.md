# Oddyssey Ecommerce

A full-stack ecommerce web application built with Node.js, Express, MongoDB, and React. This project supports user authentication, product management, cart, checkout, and admin features. Now with Docker support for easy deployment!

## Features

- User authentication (register, login, forgot password)
- Admin dashboard for managing products and categories
- Product catalog, search, and filtering
- Shopping cart and checkout with Stripe integration
- Responsive UI with React
- RESTful API with Express
- MongoDB for data storage
- Docker support for backend

## Tech Stack

- **Frontend:** React, Tailwind CSS
- **Backend:** Node.js, Express
- **Database:** MongoDB
- **Authentication:** JWT
- **Payments:** Stripe
- **Containerization:** Docker

## Project Structure

```
oddyssey-ecommerce/
  client/           # React frontend
  config/           # Database config
  controllers/      # Express controllers
  helpers/          # Helper functions
  middlewares/      # Express middlewares
  models/           # Mongoose models
  routes/           # Express routes
  index.js          # Express app entry point
  Dockerfile        # Docker config for backend
  .dockerignore     # Docker ignore file
  .env              # Environment variables
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_GITHUB_USERNAME/YOUR_REPO_NAME.git
cd oddyssey-ecommerce
```

### 2. Install dependencies

```bash
npm install
cd client && npm install
```

### 3. Set up environment variables

Create a `.env` file in the root directory:

```
MONGODB_URL=mongodb://localhost:27017/oddyssey-ecommerce
JWT_SECRET=your_jwt_secret_key
PORT=5000
```

### 4. Run the app locally

- **Backend:**
  ```bash
  npm run server
  ```
- **Frontend:**
  ```bash
  cd client
  npm start
  ```

## Docker Usage

### Build and Run with Docker

1. Build the Docker image:
   ```bash
   docker build -t oddyssey-ecommerce-backend .
   ```
2. Run the container (make sure MongoDB is running on your host):
   ```bash
   docker run -p 5000:5000 --env-file .env oddyssey-ecommerce-backend
   ```

## Environment Variables

- `MONGODB_URL` - MongoDB connection string
- `JWT_SECRET` - Secret for JWT authentication
- `PORT` - Server port (default: 5000)

Crafted with a dash of curiosity, a sprinkle of caffeine, and a whole lot of code by **Pulkit Kumar**.

If you find a bug, it's probably just a feature in disguise! 🐞✨
