# Movie Management System with REST API

## Description

Building Movie Management REST API from scratch, starting with basic CRUD operations and evolving into a sophisticated, enterprise-grade system with advanced features.

This project is a RESTful API developed with .NET Core, designed to manage movie data efficiently. It supports creating, reading, updating, and deleting movies, as well as handling user ratings. The API incorporates modern practices such as authentication, API versioning, and performance optimization, making it a robust and scalable solution. Additionally, a client SDK built with Refit provides a type-safe interface for consuming the API in .NET applications.

## Features

- **CRUD Operations**: Create, read, update, and delete movie records with a user-friendly API.
- **User Ratings**: Enable users to submit and retrieve movie ratings, calculating averages dynamically.
- **Authentication and Authorization**: Secure endpoints using JSON Web Tokens (JWT) to restrict access to authorized users.
- **API Versioning**: Support multiple API versions to ensure backward compatibility and smooth updates.
- **Output Caching**: Enhance performance by caching frequently accessed data, reducing server load.
- **Swagger Documentation**: Provide interactive API documentation for easy exploration and testing.
- **Client SDK**: Offer a type-safe SDK built with Refit for seamless API consumption in .NET applications.

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/OmarMegahed1/Movie-Management-System-With-REST-API.git
   ```

2. **Navigate to the project directory**:
   ```bash
   cd Movie-Management-System-With-REST-API
   ```

3. **Restore dependencies**:
   ```bash
   dotnet restore
   ```

4. **Set up the database** (if applicable):
   - Update the connection string in `appsettings.json` to point to your database.
   - Apply migrations to create the database schema:
     ```bash
     dotnet ef database update
     ```

5. **Run the application**:
   ```bash
   dotnet run
   ```

## Usage

- The API is accessible at `http://localhost:5000` (or the port specified in your configuration).
- Use tools like Postman or curl to interact with the API endpoints.
- Explore the interactive Swagger documentation at `/swagger` for detailed endpoint information and testing.

## API Endpoints

| Method | Endpoint                     | Description                          |
|--------|------------------------------|--------------------------------------|
| GET    | `/api/movies`               | Retrieve a list of all movies        |
| GET    | `/api/movies/{id}`          | Retrieve a specific movie by ID      |
| POST   | `/api/movies`               | Create a new movie                   |
| PUT    | `/api/movies/{id}`          | Update an existing movie             |
| DELETE | `/api/movies/{id}`          | Delete a movie                       |
| POST   | `/api/movies/{id}/ratings`  | Add a rating to a movie              |
| POST   | `/api/auth/login`           | Authenticate and receive a JWT token |

## License

This project is licensed under the [MIT License](LICENSE).
