# Habit Tracker

**Habit Tracker** is a web application developed with **ASP.NET Core** and **Entity Framework Core**. This application enables users to manage and track their habits, providing CRUD functionality (Create, Read, Update, Delete) for habit entries. Users can add new habits, update existing ones, view their habit progress, and delete habits.

## Features

- **Add Habit**: Users can create a new habit with relevant details.
- **View Habits**: List all habits with their details and tracking status.
- **Update Habit**: Users can modify habit details, including name and description.
- **Delete Habit**: Remove any habit from the tracking list.

## Tech Stack

- **Backend**: ASP.NET Core with Entity Framework Core for database management
- **Database**: SQLite or SQL Server (configured in `appsettings.json`)
- **Frontend**: HTML/CSS with Razor Pages or MVC pattern
- **Tools**: Git for version control, Dependency Injection, and built-in .NET libraries

## Project Structure

- **Controllers**: Contains all controllers handling HTTP requests and routing for CRUD operations.
- **Models**: Defines data models, including `Habit` and any other entities involved.
- **Data**: Manages database context using Entity Framework Core.
- **Views**: Razor views for displaying and interacting with habits.
- **wwwroot**: Static files, including CSS and JavaScript, for the frontend.

## Installation and Setup

### Prerequisites

- **.NET Core SDK** (3.1 or later)
- **SQL Server** (or use SQLite as default)

### Steps

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/Habit-Tracker.git
   cd Habit-Tracker
 
2. **Configure Database**:
- Adjust the database settings in `appsettings.json` or `appsettings.Development.json`.
- Ensure that Entity Framework Core migrations are updated.

 3. **Run Migrations**:
 ```bash
 dotnet ef database update
 ```

4. **Start the Application**
 ```bash
 dotnet run
 ```

The application will be running on [http://localhost:5000](http://localhost:5000) by default.

## Usage

- **Access the Habit Tracker**: Navigate to [http://localhost:5000](http://localhost:5000) in your web browser.
- **Add a New Habit**: Use the form provided to add a habit with its details.
- **Edit/Delete Habit**: Manage your habits by updating or removing entries as needed.
