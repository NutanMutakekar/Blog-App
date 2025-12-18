#Blog App API

A simple **Blog Application REST API** built using **Node.js**, **Express**, and **MongoDB**.  
This backend provides CRUD operations for blog posts and uses a modular folder structure.

---

## 🚀 Features

- Create, Read, Update, Delete blog posts  
- Structured MVC-style architecture  
- Centralized database connection  
- Custom error handling middleware  
- Routes organized by functionality

---

## 🛠 Tech Stack

| Technology | Purpose |
|------------|---------|
| Node.js | Runtime environment |
| Express | HTTP server & routing |
| MongoDB | Database |
| Mongoose | ODM for MongoDB |
| npm | Package manager |

---

## 📁 Project Structure

Blog-App/
├─ AppError/ # Custom error classes
├─ controllers/ # Request handlers
├─ middleware/ # Custom middleware (error handling, validation etc.)
├─ models/ # Mongoose schema models
├─ routes/ # Express route definitions
├─ db.js # MongoDB connection setup
├─ index.js # App entrypoint (server setup)
├─ package.json # Dependencies & scripts
└─ .gitignore



---

## 🧩 Pre-requisites

Before running this project, ensure:

✔ Node.js & npm are installed  
✔ MongoDB is running locally or you have a cloud URI (e.g., MongoDB Atlas)

---

## ⚙️ Installation

1. **Clone the repository**
   git clone https://github.com/NutanMutakekar/Blog-App.git
Navigate into the project

cd Blog-App

Install dependencies
npm install

Create environment variables
Create a .env file in the root (if using env vars):

Setup Database
MONGO_URI=your_mongodb_connection_string
PORT=5000
Start the server

npm start
Or if you prefer using nodemon:

npm run dev

📡 API Endpoints
Example endpoints — rename/update based on your actual route paths

Method	Route	Description
GET	/api/posts	Retrieve all blog posts
GET	/api/posts/:id	Retrieve a blog post by ID
POST	/api/posts	Create a new blog post
PUT	/api/posts/:id	Update an existing blog post
DELETE	/api/posts/:id	Delete a blog post

🧠 Error Handling
This API uses custom error classes and centralized middleware in middleware/ to return formatted JSON error responses for:

✔ Resource not found
✔ Validation failures
✔ Server errors

🧪 Testing
You can test the API using tools like:

Postman

Insomnia

cURL

🧑‍💻 Contributing
If you’d like to contribute:

Fork the repository

Create a new branch (git checkout -b feature-name)

Make changes

Open a pull request

📜 License
This project is open-source and licensed under the MIT License.

🙌 Acknowledgements
Thanks for exploring this project — feel free to customize the API and add features like authentication, comments, and pagination!
