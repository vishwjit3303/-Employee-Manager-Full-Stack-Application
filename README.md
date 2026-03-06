
# 🧑‍💼 Employee Manager – Full Stack Application

A Full-Stack Employee Management System built with Angular 14 (Frontend) and ASP.NET Core 6 Web API (Backend) with SQL Server Database.

This project demonstrates a complete CRUD (Create, Read, Update, Delete) workflow for managing employee records.

![Angular](https://img.shields.io/badge/Angular-14.0.5-DD0031?style=for-the-badge&logo=angular)
![TypeScript](https://img.shields.io/badge/TypeScript-4.7.2-3178C6?style=for-the-badge&logo=typescript)
![.NET](https://img.shields.io/badge/.NET-6.0-512BD4?style=for-the-badge&logo=.net)
![SQL Server](https://img.shields.io/badge/SQLServer-Database-CC2927?style=for-the-badge&logo=microsoftsqlserver)

---

# 📋 Overview

Employee Manager is a web application where users can:

- View employee records
- Add new employees
- Update employee details
- Delete employees

The system uses:

- Angular 14 for the UI
- ASP.NET Core Web API for backend services
- Entity Framework Core for database operations
- SQL Server database

---

# 🏗 Project Architecture

Angular Frontend  →  ASP.NET Core API  →  SQL Server Database

---

# 🛠 Tech Stack

| Layer | Technology |
|------|-------------|
| Frontend | Angular 14 |
| Language | TypeScript |
| Backend | ASP.NET Core 6 |
| ORM | Entity Framework Core |
| Database | SQL Server |
| API Docs | Swagger |

---

# 📁 Project Structure

EmployeeManager/

Frontend

Angular_UI-frontend/
- Components
- Models
- Services
- Routing
- Environment Config

Backend

ASP_API/
- Controllers
- Models
- DbContext
- Migrations
- Configuration

---

# ✨ Features

- View Employees
- Add Employee
- Edit Employee
- Delete Employee
- REST API Integration
- Angular Routing
- Swagger API Testing

---

# 📦 Prerequisites

Install the following:

- Node.js
- npm
- Angular CLI
- .NET 6 SDK
- SQL Server
- Visual Studio / VS Code

Install Angular CLI:

npm install -g @angular/cli@14

---

# ⚙️ Backend Setup

cd ASP_API

dotnet restore

Update connection string in appsettings.json

Run migration:

dotnet ef migrations add InitialCreate
dotnet ef database update

Run API:

dotnet run

API runs at:

https://localhost:7045

Swagger:

https://localhost:7045/swagger

---

# ⚙️ Frontend Setup

cd Angular_UI-frontend

npm install

Run Angular app:

ng serve

Open browser:

http://localhost:4200

---

# 🔌 API Endpoints

GET /api/employee → Get all employees

GET /api/employee/{id} → Get employee by id

POST /api/employee → Add employee

PUT /api/employee → Update employee

DELETE /api/employee/{id} → Delete employee

---

# 👤 Employee Model

Id : GUID

Name : string

Father : string

Email : string

Salary : int

Sex : string

Department : string

Password : string

---

# 🧭 Angular Routes

/home → Home Page

/employee → Employee List

/add → Add Employee

/edit/:id → Edit Employee

---

# 🔍 Troubleshooting

CORS Error

Enable CORS in Program.cs

app.UseCors(policy =>
    policy.AllowAnyOrigin()
          .AllowAnyHeader()
          .AllowAnyMethod());

---

Port already in use

ng serve --port 4300

---

## Here is a sample screenshots,




![list](https://user-images.githubusercontent.com/84455217/188958694-c5426148-7c27-4a01-b7ce-f66bdecf2c55.png)



<br>




![update and delete](https://user-images.githubusercontent.com/84455217/188958729-60a77b5b-419a-442e-9ee1-9a79bd1a70eb.png)




<br>



![add](https://user-images.githubusercontent.com/84455217/188958737-4704a1a2-30dd-4cc6-acd4-42d93782cc11.png)



<br>



# ⚠️ Known Issues

- Password stored in plain text
- Update API not async

---

# 📄 License

This project is for educational purposes.

---

# 👨‍💻 Author

Vishwajit

Full Stack Developer (Angular + ASP.NET Core)
