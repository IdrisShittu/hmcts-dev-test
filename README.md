# HMCTS Task Management Application

This is a full-stack task management system built for the HMCTS Developer Test. It combines a React frontend and a Spring Boot backend to support the creation, viewing, updating, and deletion of tasks.

---

## 📁 Project Structure
```
/hmcts-dev-test-main/
├── hmcts-dev-test-backend-master/   # Spring Boot backend API
└── hmcts-dev-test-frontend-main/    # React frontend app
```

---

## 🚀 Getting Started

### 🔧 Prerequisites
- Java 21+
- Gradle (or use included wrapper)
- Node.js & npm

---

## 🔙 Backend (Spring Boot)

### 📦 Build and Run
```bash
cd hmcts-dev-test-backend-master
./gradlew build
./gradlew bootRun
```
Access it via: `http://localhost:4000`

### 🔗 API Endpoints
- `GET /tasks` – Retrieve all tasks
- `POST /tasks` – Create a new task
- `GET /tasks/{id}` – Get a task by id
- `PATCH /tasks/{id}/status` – Update task status
- `DELETE /tasks/{id}` – Delete a task

### 📘 API Docs
- Swagger UI: [http://localhost:4000/swagger-ui.html](http://localhost:4000/swagger-ui.html)
- OpenAPI Docs: [http://localhost:4000/v3/api-docs](http://localhost:4000/v3/api-docs)

### 🗃️ H2 Database Console
- [http://localhost:4000/h2-console](http://localhost:4000/h2-console)
- JDBC URL: `jdbc:h2:mem:testdb`
- Username: `sa`
- Password: `password`

---

## 🖥️ Frontend (React)

### ▶️ Start Frontend
```bash
cd hmcts-dev-test-frontend-main
cd frontend
npm install
npm start
```
Frontend runs on: `http://localhost:3000`

### ✨ Features
- Create tasks with title, description, status, and due date
- View list of tasks
- Update task status
- Delete tasks
- Includes loading spinner and toast notifications

---

## ✅ Running Tests

### Backend
```bash
cd backend
./gradlew test
```

### Frontend
```bash
cd frontend
npm test
```

---

## 📄 License
MIT License

