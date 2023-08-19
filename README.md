# Request Header Parser Microservice

Build a full stack JavaScript app that is functionally similar to this: https://request-header-parser-microservice.freecodecamp.rocks/. 

This code is for a Node.js application that sets up a basic API using the Express.js framework. The application provides a single API endpoint called "/api/whoami" that returns information about the client's IP address, language, and user agent software. Here's an explanation of the code:

Module Imports:

The dotenv module is imported to load environment variables from a .env file.
The express and cors modules are imported to create the server and enable Cross-Origin Resource Sharing (CORS).
Loading Environment Variables:

Any environment variables defined in the .env file are loaded using dotenv.
Express Application Initialization:

An instance of the Express application is created using express().
CORS Configuration:

CORS is enabled using the cors middleware to allow remote testing of the API.
Legacy browsers that might have issues with a 204 response are sent a 200 status.
Static File Serving:

The application serves static files located in the "public" directory. This is useful for serving client-side files like CSS, images, and JavaScript.
Basic Routing:

When a request is made to the root route ("/"), the server sends the "index.html" file located in the "views" directory.
User Information API Endpoint:

An API endpoint (/api/whoami) is created to handle requests for user information.
The client's IP address is obtained through req.socket.remoteAddress.
The language is obtained from the "accept-language" header of the request.
The user agent software is obtained from the "user-agent" header of the request.
The server responds with a JSON object containing this information.
Server Listening:

The server starts listening on the port specified in the process.env.PORT variable or on port 3000 if not provided.
A message is logged to indicate that the server is running and listening on the specified port.
In summary, this code creates a simple Express.js application that provides an API endpoint to fetch information about the client's IP address, language, and user agent software. It's an example of how to build a basic API to gather client data using Node.js and Express.js.

# Author

- Author - [@AndresF-SanchezG](https://github.com/AndresF-SanchezG)
- School - [Freecodecamp](https://www.freecodecamp.org/)
- Curse - [Request Header Parser Microservice](https://www.freecodecamp.org/learn/back-end-development-and-apis/back-end-development-and-apis-projects/request-header-parser-microservice)






