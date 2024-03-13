# Secrets-Project
To use this code, first, install the required packages by running 'npm install' in your terminal. Then, start the application using 'nodemon index.js'.

This code sets up a simple web application using the Express framework in Node.js. It includes a basic authentication mechanism for accessing a secret page. Here's a breakdown of the code:

1. Import necessary modules: The code imports the required modules, such as Express and bodyParser, which helps parse incoming request bodies.

2. Set up the Express application: The code initializes the Express application and assigns a port number (3000) for the server to listen on.

3. Define a user authorization flag: A global flag named `userIsAuthorised` is set to `false` initially. This flag will be used to determine if the user has successfully authenticated.

4. Configure middleware: The code uses `bodyParser.urlencoded` as middleware to parse URL-encoded data from incoming requests.

5. Define a password check function: This function, `passwordCheck`, checks if the password provided in the request body matches the string "ILoveProgramming". If it does, the `userIsAuthorised` flag is set to `true`.

6. Apply password check middleware: The password check function is applied as middleware using `app.use`, so it will be executed for each incoming request.

7. Set up routes: The application has two routes:

   a. GET request to the root path ("/"): This route sends the "index.html" file from the "public" folder.
   
   b. POST request to the "/check" path: This route checks the `userIsAuthorised` flag. If it's `true`, it sends the "secret.html" file. If it's `false`, it sends the "index.html" file (or you can also use `res.redirect("/")` to redirect the user to the root path).

8. Start the server: The server listens on the specified port (3000) and logs a message when it starts.

In summary, this code sets up a basic Express application with a simple password-based authentication system to access a secret page.
