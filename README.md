<h1>Full-Stack Social Media App-Mern</h1>

This is a full-stack web application designed to demonstrate key concepts in modern web development, including user authentication, post management, and robust data handling. It features a Node.js/Express backend with MongoDB, and a React frontend 

<h2>Purpose</h2>

This project is for demonstrative purposes only and is not intended for real-world, production-grade use.

It showcases a full-stack social media application built with a Node.js/Express backend and a React/TypeScript frontend. The application's architecture emphasizes data integrity and consistency by using MongoDB transactions for critical operations like post creation, user deletion, and post interactions. This ensures that related database updates either all succeed or all fail together, maintaining a reliable state.

Security is handled through bcrypt for password hashing, jsonwebtoken for session management, and DOMPurify for sanitizing user-generated content against XSS attacks.

<h2>Features</h2>
User Authentication: Secure registration, login, and logout using JWT.
User Management: Change password, delete account (with post anonymization).
Post Management: Create, view, and delete posts.
Post Interaction: Like and unlike posts.
Dynamic Content Loading: Posts are fetched with infinite scrolling/pagination.
User Avatars: Automatically generated avatars for users.
Input Validation: Client-side and server-side validation for user inputs.
<h2>Technologies</h2>

Backend
Node.js & Express.js
MongoDB Atlas (Database) & Mongoose (ODM)
bcrypt (Password hashing)
jsonwebtoken (JWT for authentication)
DOMPurify (HTML sanitization)
Frontend
React & TypeScript
Chakra UI (Component library)
Vite (Build tool)
Axios (HTTP client)
Getting Started
Follow these steps to set up and run the project locally.

<h2>Clone the repository:</h2>

Backend Setup: Navigate to the server directory and install dependencies:

cd server
npm install
Create a .env file in the server directory with the following content:

ATLAS_URI="your_mongodb_connection_string"
JWT_SECRET="a_very_long_and_random_secret_key_for_jwt"
Replace "your_mongodb_connection_string" with your MongoDB Atlas connection string.
Replace "a_very_long_and_random_secret_key_for_jwt" with a strong, random string.
Start the backend server:

npm run dev

The server will run on https://localhost:3443.

Frontend Setup: Open a new terminal, navigate back to the project root, and then into the client directory:

cd ..
cd client
npm install
Create a .env file in the client directory with the following content:

VITE_API_BASE_URL="https://localhost:3443/api"
This tells the frontend where to find your backend API.

<h2>Start the frontend development server:</h2>

npm run dev
The frontend will typically run on http://localhost:5173.

<h2>License</h2>
This project is provided under the MIT License. See the LICENSE file in the repository root for details
