##Modern Task Manager
A professional, full-stack inspired Task Management Dashboard built with React and Tailwind CSS. This application features a robust authentication system, real-time task filtering, and a simulated API backend using Browser LocalStorage.

## Made by 
Shubham Sharma 

KJSC SOMAIYA MTECH : shubham26@somaiya.edu

CSE

## Features
1) Secure Authentication: Complete Login and Registration flow with form validation and persistent sessions.

2) Full CRUD Operations: Create, Read, Update, and Delete tasks with a smooth modal interface.

3) Task Categorization: Manage tasks by Priority (Low, Medium, High) and Status (Pending, In Progress, Completed).

4) Real-time Search & Filter: Instantly find tasks using the search bar or filter by status categories.

5) Responsive UI: Clean, mobile-friendly design using Tailwind CSS and Lucide-React icons.

6) Mock API Layer: Simulated asynchronous API calls with loading states to mimic real-world network behavior.

## Technical Stack
1) Frontend: React (Hooks, Context API)

2) Styling: Tailwind CSS (JIT mode)

3) Icons: Lucide-React

4) State Management: React Context (Global Auth state)

5) Storage: LocalStorage API

## Architecture Overview
1) The application is built with a modular architecture to ensure the codebase remains clean and scalable:

2) Auth Context: Centralizes the global user state. It provides login, register, and logout methods to all components via the useAuth hook.

3) API Service Layer: A specialized api object that intercepts requests. It simulates database latency and manages data persistence in localStorage.

4) UI Components: Atomic, reusable components (Button, Input, Alert) designed for design consistency and accessibility.

5) Conditional Routing: A top-level logic gate that checks the authentication status to serve either the Auth pages or the Dashboard.

<img width="635" height="675" alt="image" src="https://github.com/user-attachments/assets/ef5bee4d-1cd3-4080-91ef-a347e751950a" />


<img width="1564" height="731" alt="image" src="https://github.com/user-attachments/assets/fcbc779e-db9a-47a7-9754-33861d204222" />


Filter 

<img width="1573" height="740" alt="image" src="https://github.com/user-attachments/assets/4f73f9f9-7f87-42db-bf8b-a403da5f6b51" />

<img width="1568" height="721" alt="image" src="https://github.com/user-attachments/assets/6415b02d-739a-46b4-9931-968d2109e51f" />

<img width="492" height="187" alt="image" src="https://github.com/user-attachments/assets/d1476f16-7795-42ad-a6f8-f76e94b2a7a4" />

Task deleted 

<img width="1571" height="690" alt="image" src="https://github.com/user-attachments/assets/30eb0ac0-499c-44be-a071-5671b0bf1323" />




# API Endpoints 
<img width="655" height="186" alt="image" src="https://github.com/user-attachments/assets/125c7b58-e924-4497-9e5e-0d14efd2a940" />


## Project Structure
<img width="742" height="204" alt="image" src="https://github.com/user-attachments/assets/2db97ecf-4e77-46f5-ba27-a9979d37a0bc" />


## Usage Note
This application currently uses LocalStorage for data persistence. This means your tasks and login session will persist even if you refresh the page, but they are unique to your specific browser and device.
