
---

# 📘 Blog Post Manager (MERN-style Architecture with Express)

This is a simple blog post management web application that allows users to create, read, update, and delete blog posts. It includes two servers:

* **API Server (Port 4000)** – Handles all data operations using Express.
* **Frontend Server (Port 3000)** – Renders pages using EJS and communicates with the API server via Axios.

---

## 🚀 Features

* View all blog posts
* Create a new post
* Edit an existing post
* Delete a post
* RESTful API design
* In-memory data store

---

## 🛠️ Technologies Used

* **Frontend:** EJS templating, HTML/CSS
* **Backend:** Node.js, Express.js, Axios
* **Middleware:** Body-parser
* **Templating Engine:** EJS

---

## 📁 Project Structure

```
project-root/
├── public/             # Static files (CSS, images, etc.)
├── views/              # EJS templates (index.ejs, modify.ejs)
├── server.js           # Frontend server (renders pages, handles forms)
├── api.js              # Backend server (API with in-memory DB)
├── package.json        
└── README.md           
```

---

## 🧪 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/blog-post-manager.git
cd blog-post-manager
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Start the API Server (Port 4000)

```bash
node api.js
```

### 4. Start the Frontend Server (Port 3000)

```bash
node server.js
```

---

## 🌐 Access the App

Open your browser and visit:

```
http://localhost:3000
```

---

## 📌 API Endpoints (Port 4000)

### Get all posts

```
GET /posts
```

### Get a specific post

```
GET /posts/:id
```

### Create a new post

```
POST /posts
Body: { title, content, author }
```

### Update a post (partial)

```
PATCH /posts/:id
Body: { title?, content?, author? }
```

### Delete a post

```
DELETE /posts/:id
```

---

## 📝 Frontend Routes (Port 3000)

| Route                   | Description                         |
| ----------------------- | ----------------------------------- |
| `/`                     | Display all blog posts              |
| `/new`                  | Form to create a new post           |
| `/edit/:id`             | Form to edit an existing post       |
| `/api/posts`            | Create a new post (form submission) |
| `/api/posts/:id`        | Update a post (form submission)     |
| `/api/posts/delete/:id` | Delete a post                       |

---

## 🔧 To-Do / Improvements

* Persist data using MongoDB or another database
* Add user authentication
* Implement client-side validation
* Add search/filter functionality

---

