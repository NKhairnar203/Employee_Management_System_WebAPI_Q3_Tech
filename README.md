# Employee Management System Web API

## 📌 Project Overview
The **Employee Management System Web API** is a .NET Core-based RESTful API that allows managing employees and users. It provides authentication, CRUD operations, and role-based access control.

## 📂 Project Structure
```
Employee_Management_System_API/
│── Controllers/
│   ├── AuthController.cs
│   ├── EmployeeController.cs
│── Data/
│   ├── ApplicationDbContext.cs
│── DTOs/
│   ├── UserLoginDTO.cs
│   ├── UserRegisterDTO.cs
│── Helpers/
│   ├── JwtHelper.cs
│── Migrations/
│── Models/
│   ├── Employee.cs
│   ├── User.cs
│── Repositories/
│   ├── EmployeeRepository.cs
│   ├── UserRepository.cs
│── Services/
│── appsettings.json
│── Program.cs
```

## 🚀 Features
✅ User Authentication (JWT-based)
✅ Role-based Authorization
✅ Employee CRUD Operations (Create, Read, Update, Delete)
✅ User Management
✅ Secure Password Hashing
✅ Entity Framework Core Integration
✅ Exception Handling & Validation

## 🏗️ Object-Oriented Programming (OOP) Concepts Used
### 🔹 **Encapsulation**
- Used in models like `Employee` and `User` to restrict direct access to data.

### 🔹 **Abstraction**
- Implemented using interfaces like `IEmployeeRepository` and `IUserRepository`.

### 🔹 **Inheritance**
- `BaseEntity` class can be used for common properties like `Id`, `CreatedAt`.

### 🔹 **Polymorphism**
- Dependency injection allows different repository implementations.

## 🔧 Setup & Installation
1️⃣ **Clone the Repository:**
```sh
git clone https://github.com/YourUsername/Employee_Management_System_API.git
cd Employee_Management_System_API
```
2️⃣ **Install Dependencies:**
```sh
dotnet restore
```
3️⃣ **Set Up Database:**
```sh
dotnet ef migrations add InitialCreate
dotnet ef database update
```
4️⃣ **Run the Application:**
```sh
dotnet run
```

## 🔑 API Endpoints
### 🔹 Authentication
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST | `/api/auth/register` | Register a new user |
| POST | `/api/auth/login` | Login and get JWT token |

### 🔹 Employees
| Method | Endpoint | Description |
|--------|---------|-------------|
| GET | `/api/employees` | Get all employees |
| GET | `/api/employees/{id}` | Get employee by ID |
| POST | `/api/employees` | Add a new employee |
| PUT | `/api/employees/{id}` | Update employee |
| DELETE | `/api/employees/{id}` | Delete employee |



