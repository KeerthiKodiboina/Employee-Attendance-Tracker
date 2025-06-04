# Employee-Attendance-Tracker
This project is a role-based attendance management system developed using Spring Boot, Spring Security, and PostgreSQL. It enables employees to mark their attendance and allows managers to view detailed attendance records for both individuals and departments.

A simple Spring Boot application to manage employee attendance with role-based access control. The system enables employees to mark attendance and allows managers to view detailed attendance reports by employee or department.

---

##  Features

- Add employee details
- Mark daily attendance (Present/Absent)
- View attendance per employee or department
- Role-based security with Spring Security
- RESTful API endpoints for all operations

---

##  Tech Stack

- Java 17+
- Spring Boot
- Spring Security
- Spring Data JPA
- PostgreSQL
- REST APIs

---

##  User Roles

| Role     | Username | Password |
|----------|----------|----------|
| Employee | employee | pass     |
| Manager  | manager  | pass     |

---

##  API Endpoints

###  Employee
- `POST /api/employees` – Add a new employee (MANAGER only)

###  Attendance
- `POST /api/attendance` – Mark attendance (EMPLOYEE only)
- `GET /api/attendance/employee/{id}` – View attendance by employee (MANAGER only)
- `GET /api/attendance/department/{dept}` – View attendance by department (MANAGER only)

---

##  Setup Instructions

1. Clone the repository  
2. Configure your PostgreSQL database in `application.properties`  
3. Run the Spring Boot application  
4. Test the endpoints using Postman or curl  

---

##  Author

Developed by [Keerthi Kodiboina]

---

