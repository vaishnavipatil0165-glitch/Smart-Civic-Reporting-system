
# 🏙️ Smart Civic Reporting System

A full-stack web application that allows citizens to report civic issues such as **potholes, garbage, damaged roads, water leakage, and other public problems**. Authorities can manage, assign, and track reported issues until they are resolved.

## 📌 Project Overview

The **Smart Civic Reporting System** connects citizens with civic authorities through an easy-to-use web application.

Citizens can:

* Register and login
* Report civic problems
* Add issue details
* Upload images
* Share the location of the issue
* Track complaint status

Administrators and workers can:

* View reported complaints
* Manage civic issues
* Assign issues to workers
* Update complaint status
* Track resolved and pending issues

## 🚀 Features

### 👤 Citizen

* User registration and login
* Secure authentication
* Report new civic issues
* Upload issue images
* Add location details
* View submitted complaints
* Track complaint status

### 👨‍💼 Admin

* Admin authentication
* View all complaints
* Manage reported issues
* Assign complaints to workers
* Monitor complaint progress
* Update issue status

### 🦺 Worker

* View assigned complaints
* Check complaint details
* Update work progress
* Mark issues as resolved

### 📍 Location & Images

* Location-based issue reporting
* Map integration
* Image upload using Cloudinary

## 🔄 Complaint Workflow

```text
Citizen Reports Issue
        ↓
Complaint Submitted
        ↓
Admin Reviews Complaint
        ↓
Complaint Assigned to Worker
        ↓
Worker Starts Work
        ↓
Issue Resolved
        ↓
Complaint Closed
```

## 🛠️ Technologies Used

### Frontend

* React.js
* JavaScript
* HTML5
* CSS3
* Leaflet / OpenStreetMap

### Backend

* Node.js
* Express.js
* REST API
* JWT Authentication
* bcryptjs

### Database

* MongoDB
* Mongoose

### Cloud Services

* Cloudinary for image storage

### Development Tools

* VS Code
* npm
* GitHub

## 📁 Project Structure

```text
smart-civic-reporting/
│
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   ├── models/
│   │   ├── routes/
│   │   └── server.js
│   │
│   ├── package.json
│   └── .env
│
├── frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── ...
│
├── README.md
└── .gitignore
```

> Folder names may vary slightly depending on the project version.

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/smart-civic-reporting.git
```

Move into the project:

```bash
cd smart-civic-reporting
```

## 🔧 Backend Setup

Open a terminal:

```bash
cd backend
```

Install dependencies:

```bash
npm install
```

Create a `.env` file inside the `backend` folder.

Example:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
FRONTEND_ORIGIN=http://localhost:5173

CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
```

**Never upload your real `.env` file or secret keys to GitHub.**

Start the backend:

```bash
npm run dev
```

The backend runs on:

```text
http://localhost:5000
```

## 💻 Frontend Setup

Open another terminal:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start the frontend:

```bash
npm run dev
```

Open the application in your browser:

```text
http://localhost:5173
```

## 🔐 Authentication

The application uses **JWT-based authentication** for secure user login.

Passwords are protected using **bcryptjs**.

Different users can have different roles, such as:

```text
Citizen
Worker
Admin
Super Admin
```

## 🗄️ Database

The project uses **MongoDB** to store application data such as:

* Users
* Complaints
* Departments
* Workers
* Issue status
* Location information

Mongoose is used to communicate between the Node.js backend and MongoDB.

## ☁️ Cloudinary

Cloudinary is used to store images uploaded with civic complaints.

For example:

```text
Citizen
   ↓
Upload Issue Image
   ↓
Cloudinary
   ↓
Image URL
   ↓
MongoDB
```

## 📍 Map Integration

The application uses **Leaflet/OpenStreetMap** for displaying and selecting locations.

This helps citizens provide the location of a civic problem.

## 🧪 Testing the Application

After starting both servers:

### Frontend

```text
http://localhost:5173
```

### Backend

```text
http://localhost:5000
```

Test the following:

* User registration
* User login
* Create complaint
* Upload image
* Add location
* View complaint
* Admin complaint management
* Worker assignment
* Complaint status updates

## 🔒 Security

The following files should not be uploaded to GitHub:

```text
.env
node_modules/
```

Recommended `.gitignore`:

```gitignore
node_modules/
.env
backend/.env
frontend/.env
dist/
build/
.vite/
```

## 🎯 Future Scope

* AI-based civic issue detection
* Automatic pothole detection using computer vision
* AI-based complaint classification
* Automatic department assignment
* Email and SMS notifications
* Mobile application
* Real-time complaint tracking
* Citizen feedback and ratings
* Analytics dashboard
* Complaint priority prediction
* Integration with smart-city IoT sensors

## 👩‍💻 Project Purpose

This project demonstrates how a **full-stack web application** can be used to improve communication between citizens and civic authorities.

It combines:

```text
React
+
Node.js
+
Express
+
MongoDB
+
JWT
+
Cloudinary
+
Maps
```

to create a centralized platform for reporting and managing civic issues.

## 📜 License

This project is intended for educational and project-development purposes.

## ⭐ Acknowledgement

This project was developed as a full-stack web application for learning and demonstrating modern web development, database management, authentication, cloud storage, and civic issue management.
