# Golang CRUD Application

## About the Project

This project is a simple CRUD (Create, Read, Update, Delete) application built with Golang and the Gin framework, designed to manage posts. It connects to a PostgreSQL database using GORM, the Go Object-Relational Mapper (ORM) library. The project demonstrates basic functionalities such as creating, retrieving, updating, and deleting posts, while also incorporating environment variable management and database migrations.

## Project Structure

- **main.go**: The entry point of the application, where routes are defined and the server is started.
- **controllers/postsController.go**: Contains the controller logic for handling CRUD operations for posts.
- **initializers/database.go**: Handles database connection using environment variables.
- **initializers/loadEnvVariables.go**: Loads environment variables from the .env file.
- **migrate/migrate.go**: Handles database migrations to create the necessary tables.
- **models/postModel.go**: Defines the Post model representing the structure of a post in the database.

## Getting Started

### Prerequisites

- Go 1.16+
- PostgreSQL

### Installation

1. Clone the repository:
    ```sh
    git clone <repository_url>
    ```
2. Navigate to the project directory:
    ```sh
    cd Golang-CRUD-main
    ```
3. Create a `.env` file and add your database URL:
    ```sh
    echo "DB_URL=your_database_url" > .env
    ```

### Running the Application

1. Load environment variables and connect to the database:
    ```sh
    go run main.go
    ```

2. Run database migrations:
    ```sh
    go run migrate/migrate.go
    ```

3. Start the server:
    ```sh
    go run main.go
    ```

The application will be running on `http://localhost:8080`.

### API Endpoints

- `POST /posts`: Create a new post
- `GET /posts`: Retrieve all posts
- `GET /posts/:id`: Retrieve a single post by ID
- `PUT /posts/:id`: Update a post by ID
- `DELETE /posts/:id`: Delete a post by ID

## Contributing

Contributions are what make the open-source community such an amazing place to be, learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE` for more information.

Alter to test config git on mac, update
