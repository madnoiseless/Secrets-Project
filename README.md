# Secrets Sharing Application

This project is a simple web application that allows users to access a collection of secrets by providing a password. The application uses Express.js for the server-side logic and serves HTML pages for the user interface.

## Prerequisites

Before starting, make sure you have the following software installed:

1. Node.js: Download and install it from [https://nodejs.org/](https://nodejs.org/)

## Installation

1. Clone the repository or download the project files.
2. Open your terminal or command prompt and navigate to the project directory.
3. Run `npm install` to install the required dependencies.

## Usage

1. Run the application using the command `node index.js`.
2. The server will start and listen on port `3000`.
3. Open your browser and navigate to `http://localhost:3000`.
4. You will be presented with a password input form.
5. Enter the password `ILoveProgramming` to access the secrets page.
6. If the password is incorrect, you will be redirected back to the login page.
7. Upon successful authentication, you will be able to view the secrets stored in `secret.html`.

## Dependencies

This project uses the following NPM packages:

1. [Express](https://www.npmjs.com/package/express): A fast, minimalist web framework for Node.js.
2. [Body-parser](https://www.npmjs.com/package/body-parser): Middleware to parse incoming request bodies in a middleware before your handlers.

## File Structure

- `index.js`: The main server file that sets up the Express application and handles routes.
- `public/index.html`: The login page where users enter the password.
- `public/secret.html`: The page containing the secrets that will be displayed upon successful authentication.

## Contributing

Contributions, issues, and feature requests are welcome! Feel free to create a pull request or submit an issue.
