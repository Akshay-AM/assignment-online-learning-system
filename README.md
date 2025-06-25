
markdown
Copy
Edit
# 🎓 Online Learning Platform

A full-stack web application that allows users to register, browse courses, enroll, learn through multimedia lessons, take quizzes, and track their progress. Developed with **Spring Boot**, **React.js**, and **MySQL**.

---

## 🚀 Features

### 🔐 User Management
- Register & Login 


### 📚 Course Management
- Create/update/delete courses
- Add lessons, quizzes, PDFs, and video materials
- Categorize and tag courses for easy browsing

### 📖 Learning & Progress
- Enroll in courses
- Track lesson, quiz, and assignment completion
- Responsive design and media support (PDF, video, etc.)

---

## 🛠 Tech Stack

| Layer      | Tech                        |
|------------|-----------------------------|
| Frontend   | React.js, HTML, CSS, Bootstrap |
| Backend    | Spring Boot, Spring Security |
| Database   | MySQL                       |
| Auth       | JWT |
| ORM        | JPA (Hibernate)             |
| API Testing| Postman                     |

---

## 🗂️ Project Structure

### Backend (`/backend`)
com.lms
├── controller
├── model
├── repository
├── service (optional)
├── config
└── Application.java

shell
Copy
Edit

### Frontend (`/frontend`)
/src
├── components
├── pages
├── services
└── App.js

yaml
Copy
Edit

---

## 🔧 Setup Instructions

### Prerequisites
- Java 17
- Node.js & npm
- MySQL Server
- Git

---

### 🖥️ Backend Setup

```bash
cd backend
./mvnw clean install
./mvnw spring-boot:run
✅ MySQL Config (in application.properties)
properties
Copy
Edit
spring.datasource.url=jdbc:mysql://localhost:3306/lms_db
spring.datasource.username=root
spring.datasource.password=your_password
🌐 Frontend Setup
bash
Copy
Edit
cd frontend
npm install
npm start
📬 API Endpoints (Sample)
Method	Endpoint	Description
POST	/api/auth/register	Register user
POST	/api/auth/login	Login user
GET	/api/courses	Get all courses
POST	/api/courses	Create new course
GET	/api/lessons/{id}	Get lesson by ID
POST	/api/quizzes	Add quiz to a lesson
POST	/api/categories	Create course category

📘 Import the provided Postman collection (postman_collection.json) to test all APIs.

🧪 Testing
Use Postman to test all endpoints.

Example JSON payloads for each module are included in the postman folder.

✅ Future Enhancements
Certificate generation on course completion

Discussion forums

Instructor dashboard analytics

Real-time quiz and exams

🤝 Contributors
👨‍💻 Akshay A M — GitHub | LinkedIn
