**📚 Library Management System (Node.js & MongoDB)**

A simple Library Management System REST API built using Node.js, Express.js, and MongoDB (Mongoose).
This project demonstrates basic CRUD operations with real-world use cases such as managing books, categories, and available copies.

**🚀 Features**

➕ Add multiple books at once

📖 View all books

🔍 Filter books by category

📅 Get books published after a specific year

🔄 Update available copies

🏷️ Change book category

❌ Delete books when copies reach zero

⚠️ Prevent negative stock

🛠️ Tech Stack

Backend: Node.js, Express.js

Database: MongoDB

ODM: Mongoose

Tools: npm, Postman

**📂 Project Structure**
├── app.js               # Main server file
├── db.js                # MongoDB connection
├── bookmodel.js         # Book schema & model
├── package.json         # Project dependencies
├── package-lock.json    # Dependency lock file
└── README.md            # Project documentation

**📦 Installation & Setup**

Clone the repository

git clone https://github.com/your-username/library-management-system.git


Navigate to project folder

cd library-management-system


Install dependencies

npm install


Start MongoDB

Make sure MongoDB is running on:

mongodb://127.0.0.1:27017/libraryDB


Run the server

node app.js


Server will run on

http://localhost:3000

🔗 API Endpoints
➕ Add Books
POST /addBooks

📖 Get All Books
GET /books

🏷️ Get Books by Category
GET /books/category/:category

📅 Books Published After 2015
GET /books/year/after2015

🔄 Update Available Copies
PUT /books/updateCopies/:id


Body:

{
  "change": 1
}

🏷️ Change Book
PUT /books/changeCategory/:id


Body:

{
  "category": "AI"
}

❌ Delete Book (Only if copies = 0)
DELETE /books/delete/:id

✅ Sample Book Model

{
  title: String,
  author: String,
  category: String,
  publishedYear: Number,
  availableCopies: Number
}

**🧠 Learning Outcomes**

REST API design

MongoDB CRUD operations

Express routing

Mongoose schema & validation

Error handling

**📌 Future Enhancements**

User authentication

Borrow & return books

Admin dashboard

Pagination & search

Environment variables (.env)

**👤 Author**

Nithila Gnanavel
B.Tech Student
Node.js | MongoDB | Backend Development
Image created
•
Library Management System README overview
