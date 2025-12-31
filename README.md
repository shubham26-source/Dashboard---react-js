Modern Task Manager
A professional, full-stack inspired Task Management Dashboard built with React and Tailwind CSS. This application features a robust authentication system, real-time task filtering, and a simulated API backend using Browser LocalStorage.

## Made by 
Shubham Sharma 
KJSC SOMAIYA MTECH 
CSE

## Features
Secure Authentication: Complete Login and Registration flow with form validation and persistent sessions.

Full CRUD Operations: Create, Read, Update, and Delete tasks with a smooth modal interface.

Task Categorization: Manage tasks by Priority (Low, Medium, High) and Status (Pending, In Progress, Completed).

Real-time Search & Filter: Instantly find tasks using the search bar or filter by status categories.

Responsive UI: Clean, mobile-friendly design using Tailwind CSS and Lucide-React icons.

Mock API Layer: Simulated asynchronous API calls with loading states to mimic real-world network behavior.

## Technical Stack
Frontend: React (Hooks, Context API)

Styling: Tailwind CSS (JIT mode)

Icons: Lucide-React

State Management: React Context (Global Auth state)

Storage: LocalStorage API

## Architecture Overview
The application is built with a modular architecture to ensure the codebase remains clean and scalable:

Auth Context: Centralizes the global user state. It provides login, register, and logout methods to all components via the useAuth hook.

API Service Layer: A specialized api object that intercepts requests. It simulates database latency and manages data persistence in localStorage.

UI Components: Atomic, reusable components (Button, Input, Alert) designed for design consistency and accessibility.

Conditional Routing: A top-level logic gate that checks the authentication status to serve either the Auth pages or the Dashboard.

# API Endpoints 
The application uses a centralized api.call(endpoint, options) method to handle data:
Endpoint,Method,Action
/auth/login,POST,Validates credentials and returns a mock JWT token.
/auth/register,POST,Creates a user profile and signs them in.
/tasks,GET,Fetches all tasks associated with the session.
/tasks,POST,Adds a new task to the database.
/tasks/:id,PUT,"Updates priority, status, or content of a task."
/tasks/:id,DELETE,Removes a task from storage.

## Project Structure
src/
├── components/     # Reusable UI elements (Button, Input, Alert)
├── context/        # AuthProvider and Context logic
├── services/       # Mock API and localStorage handlers
├── App.js          # Main routing and state logic
└── index.js        # Root entry point

## Usage Note
This application currently uses LocalStorage for data persistence. This means your tasks and login session will persist even if you refresh the page, but they are unique to your specific browser and device.
