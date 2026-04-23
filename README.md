# Flask User Management Web Application

## Overview

This project is a full-stack web application built using Flask that supports user registration, login authentication, file upload, and profile management. The application stores user data in a SQLite database and processes uploaded text files to compute word counts.

---

## Features

* User Registration and Login Authentication
* File upload support for `.txt` files
* Word count processing for uploaded files
* User profile page displaying stored details
* SQLite database integration
* Lightweight and easy to deploy

---

## Tech Stack

* **Backend:** Python (Flask)
* **Frontend:** HTML, CSS
* **Database:** SQLite
* **Deployment Ready:** AWS (EC2 with WSGI support)

---

## Project Structure

```
.
├── flaskapp.py
├── flaskapp.wsgi
├── templates/
│   ├── login.html
│   ├── registration.html
│   └── user_profile.html
├── mydatabase.db
└── uploads/
```

---

## How It Works

1. User registers with personal details
2. User uploads a `.txt` file during registration
3. The application:

   * Saves the uploaded file
   * Counts the number of words in the file
   * Stores user data and word count in the database
4. User logs in using credentials
5. Profile page displays:

   * User information
   * Word count
   * Download link for uploaded file

---

## How to Run Locally

### 1. Clone the repository

```
git clone https://github.com/kyatham-2/flask-user-management-app.git
```

### 2. Navigate to the project folder

```
cd flask-user-management-app
```

### 3. Install dependencies

```
pip install flask
```

### 4. Run the application

```
python flaskapp.py
```

### 5. Open in browser

```
http://127.0.0.1:5000/
```

---

## Key Highlights

* End-to-end full-stack application
* Demonstrates authentication flow (register → login → profile)
* Handles file uploads and processing
* Uses SQLite for persistent storage
* Simple and extendable architecture

---

## Future Improvements

* Add password hashing for security
* Improve input validation and error handling
* Restrict file size and type validation
* Use environment variables for configuration
* Add Docker support for containerization
* Deploy fully on AWS with production setup
