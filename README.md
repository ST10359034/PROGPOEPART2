# Agri-Energy Connect1 Prototype

## Project Overview
Agri-Energy Connect1 is a prototype web application designed to connect the agricultural sector with green energy technology providers. The platform enables farmers and employees to collaborate, manage products, and access resources for sustainable agriculture and renewable energy.

---

## Step-by-Step Setup Instructions

1. **Clone the Repository**
   - Download or clone the project to your local machine.

2. **Open the Project**
   - Open the solution (`AgriEnergyConnect1.sln`) in Visual Studio 2022 or later.
   - Ensure you open the project named `AgriEnergyConnect1` within the solution.

3. **Restore Dependencies**
   - Visual Studio will automatically restore NuGet packages. If not, right-click the solution and select "Restore NuGet Packages".

4. **Configure the Database**
   - Open `AgriEnergyConnect1/appsettings.json` and ensure the `DefaultConnection` string points to your desired SQLite or SQL Server LocalDB database.

5. **Apply Database Migrations**
   - In Visual Studio, set `AgriEnergyConnect1` as the startup project.
   - Open the Package Manager Console and select `AgriEnergyConnect1` as the Default Project.
   - Run:
     ```
     Update-Database
     ```
   - This will create the necessary tables and seed sample data.

6. **Run the Application**
   - Press `F5` or click the "Run" button in Visual Studio to start the application. Make sure `AgriEnergyConnect1` is set as the startup project.

---

## How to Build and Run the Prototype

- The application is built using ASP.NET Core MVC and Entity Framework Core.
- All dependencies are managed via NuGet.
- The database is automatically seeded with sample data for demonstration.
- To run the application outside Visual Studio, navigate to the `AgriEnergyConnect1` directory and use:
  ```
  dotnet run
  ```
  (Ensure you have the .NET SDK installed.)

---

## System Functionalities and User Roles

### User Roles

- **Farmer**
  - Register and log in as a Farmer.
  - Add and view their own agricultural products.
- **Employee**
  - Register and log in as an Employee.
  - Add and view farmer profiles.
  - View and filter all products listed by farmers.

### Key Functionalities

- **Authentication & Authorization**
  - Secure login system with role-based access (Farmer, Employee).
- **Product Management**
  - Farmers can add, view, and manage their products.
- **Profile Management**
  - Employees can add and view farmer profiles.
- **Product Browsing**
  - Employees can view and filter all products.
- **Responsive UI**
  - User-friendly interface built with Bootstrap.
- **Data Validation**
  - All forms include validation for data integrity.

---

## Additional Notes

- Sample data is available in `AgriEnergyConnect1/Data/SeedData.cs` for quick testing.
- The application uses SQLite by default but can be configured for SQL Server LocalDB.
- For any issues, ensure your database connection string is correct and all migrations are applied.

---

## License

For educational use only. 
