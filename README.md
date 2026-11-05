# 🎬 RazorPageMovie

[![.NET Core](https://img.shields.io/badge/.NET-8.0-512BD4?style=for-the-badge&logo=.net&logoColor=white)](https://dotnet.microsoft.com/)
[![ASP.NET Core Razor Pages](https://img.shields.io/badge/Framework-Razor%20Pages-blueviolet?style=for-the-badge&logo=framework)](https://learn.microsoft.com/en-us/aspnet/core/razor-pages/)
[![Entity Framework Core](https://img.shields.io/badge/ORM-EF%20Core-green?style=for-the-badge)](https://learn.microsoft.com/en-us/ef/core/)


A production-ready reference web application built with **ASP.NET Core Razor Pages** and **Entity Framework Core**, demonstrating clean architecture principles, robust data management, and standard Microsoft enterprise development patterns.

---

## 🚀 Key Features

* **CRUD Operations:** Complete Create, Read, Update, and Delete lifecycle management for movie entries.
* **Advanced Data Filtering & Search:** Server-side query filtering by genre and search strings using LINQ.
* **Database Management with EF Core:** Code-First migrations, DbContext configuration, and relational data modeling.
* **Input Validation & Data Annotation:** Robust server-side and client-side validation models for data integrity.
* **Responsive UI:** Clean, modern layout leveraging Bootstrap and standard scaffolding templates.

---

## 🛠️ Tech Stack & Architecture

* **Framework:** ASP.NET Core (.NET 8)
* **Architectural Pattern:** Model-View-Controller (MVC variant via **Razor Pages** page-focused model)
* **ORM:** Entity Framework Core (SQLite / SQL Server compatible)
* **UI Framework:** HTML5, CSS3, Bootstrap
* **Tooling:** Visual Studio / VS Code / .NET CLI

---

## 📂 Project Structure

The project follows standard ASP.NET Core conventions to maximize maintainability and separation of concerns:

```text
RazorPageMovie/
│
├── Data/            # Database context and initial seed data logic
├── Models/          # Domain entities and view-specific data models
├── Pages/           # Razor Pages (UI components, code-behind logic .cshtml.cs)
├── Migrations/      # Entity Framework Core database migrations history
├── wwwroot/         # Static assets (CSS, JavaScript, images)
├── Program.cs       # Application entry point, dependency injection, and middleware pipeline
└── appsettings.json # Configuration settings (connection strings, logging)
```

---

## ⚙️ Getting Started
Follow these instructions to set up and run the project locally on your machine.

## Prerequisites
- .NET 8.0 SDK installed on your system.

## Installation & Execution
### 1. Clone the repository:
```bash
git clone https://github.com/jluisvacan/RazorPageMovie.git
cd RazorPageMovie
```

### 2. Restore dependencies:
```bash
dotnet restore
```

### 3. Apply Database Migrations (if applicable):
```bash
dotnet ef database update
``` 

### 4. Run the application:
```bash
dotnet run
```

### 5. Access the app:
```text
Open your browser and navigate to https://localhost:5256
```

## 📈 Engineering Highlights & Best Practices
- **Dependency Injection:** Built-in Microsoft IoC container utilized for clean service lifecycle management.

- **Asynchronous Programming:** Extensive use of async/await patterns for database queries to ensure high throughput and scalability.

- **Separation of Concerns:** Isolation of business logic in code-behind files (.cshtml.cs) away from markup view presentations (.cshtml).