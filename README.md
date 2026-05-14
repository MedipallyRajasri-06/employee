# Employee Management System

## Project Structure

The project is divided into two main directories:

- `employee-backend`: The Node.js and Express backend REST API.
- `frontend`: The React frontend application built with Vite.
- `req.http`: A file containing HTTP requests for testing the backend API using tools like the VS Code REST Client extension.

## Backend (`employee-backend`)

The backend is built with Node.js and Express.js, providing a RESTful API for managing employee records.

### Features

- **CRUD Operations**: Create, Read, Update, and Delete employee records.
- **Database**: MongoDB integration using Mongoose for object data modeling.
- **Authentication/Security**: Includes `bcrypt` for password hashing and `jsonwebtoken` for secure token-based authentication.
- **CORS**: Configured to allow cross-origin requests from the frontend.

### API Endpoints

Base URL: `http://localhost:4000/emp-api`

- `POST /employees`: Create a new employee.
- `GET /employees`: Retrieve all employees.
- `PUT /employees/:id`: Update an employee by ID.
- `DELETE /employees/:id`: Delete an employee by ID.

### Setup and Running

1. Navigate to the backend directory:
   ```bash
   cd employee-backend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Set up environment variables in a `.env` file (e.g., `PORT=4000`, MongoDB connection string, JWT secret).
4. Start the server:
   ```bash
   npm start
   ```

## Frontend (`frontend`)

The frontend is a modern React application bootstrapped with Vite, offering a fast and responsive user interface.

### Features

- **State Management**: Uses `zustand` for lightweight and efficient global state management.
- **Routing**: Client-side routing implemented with `react-router`.
- **Form Handling**: Form validation and submission handled smoothly with `react-hook-form`.
- **Styling**: Styled beautifully with modern utility classes using `@tailwindcss/vite` and `tailwindcss`.
- **API Calls**: Uses `axios` for making HTTP requests to the backend API.

### Setup and Running

1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```

## Getting Started

To run the full application locally, you will need to start both the backend server and the frontend development server simultaneously in separate terminal windows. Ensure your MongoDB database is running and the connection string is correctly configured in the backend's `.env` file.
