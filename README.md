# Kanban Board Application with JWT Authentication

## Description

This project is a full-stack Kanban board application where users can securely log in, manage their work tasks, and maintain authenticated access to their tasks using **JSON Web Tokens (JWTs)**. The application provides a secure login page, JWT-based authentication, and allows users to interact with a Kanban board to manage tasks effectively.

## User Story

As a member of an agile team, I want a Kanban board with a secure login page so that I can securely access and manage my work tasks.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Technologies](#technologies)
- [Features](#features)
- [Bonus Features](#bonus-features)
- [Contributing](#contributing)
- [License](#license)
- [Deployed Application](#deployed-application)
- [Screenshots](#screenshots)

## Installation

1. Clone the repository to your local machine:
    ```bash
    git clone https://github.com/your-username/kanban-jwt-app.git
    ```

2. Navigate to the project directory:
    ```bash
    cd kanban-jwt-app
    ```

3. Install server-side dependencies:
    ```bash
    cd server
    npm install
    ```

4. Install client-side dependencies:
    ```bash
    cd ../client
    npm install
    ```

5. Create a `.env` file in the `server` directory and add the following variables:
    ```bash
    DATABASE_USER=your_db_username
    DATABASE_PASSWORD=your_db_password
    JWT_SECRET=your_secret_key
    ```

6. Start the server:
    ```bash
    cd ../server
    npm start
    ```

7. Start the client:
    ```bash
    cd ../client
    npm start
    ```

8. The app will be available on `http://localhost:3000`.

## Usage

### Login and JWT Authentication

1. Navigate to the login page.
2. Enter your valid username and password.
3. Upon successful authentication, a JWT will be generated and stored in local storage, allowing you to securely access the Kanban board.
4. If the username or password is incorrect, an error message will be displayed.
5. The token will be automatically removed from local storage upon logging out.

### Kanban Board

- Once logged in, you can manage your work tasks by creating, updating, and deleting Kanban board tickets.
- Tasks are categorized into columns such as "To Do," "In Progress," and "Done."

## Technologies

### Backend

- **Node.js**: JavaScript runtime for the server.
- **Express**: Web framework for Node.js.
- **PostgreSQL**: Relational database for task and user management.
- **jsonwebtoken (JWT)**: For secure token-based authentication.

### Frontend

- **React**: Library for building the user interface.
- **Axios**: To handle HTTP requests between the client and server.
- **Bootstrap**: For a clean, responsive UI design.

## Features

- Secure authentication using JWT.
- Login and logout functionality.
- JWT stored securely in local storage for subsequent authenticated requests.
- Full Kanban board functionality with tasks in different stages.
- Protection of Kanban routes—only authenticated users can access the board.
- Automatic session expiration after a period of inactivity.

## Bonus Features

- Sorting and filtering functionality for Kanban tickets.

## Contributing

Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch:
    ```bash
    git checkout -b feature-branch
    ```
3. Make your changes and commit them:
    ```bash
    git commit -m "Your message"
    ```
4. Push to the branch:
    ```bash
    git push origin feature-branch
    ```
5. Submit a pull request.

## License

This project is licensed under the MIT License.

## Deployed Application

You can view the deployed application at: [https://your-app-url-on-render.com](https://your-app-url-on-render.com)


