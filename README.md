# Session Authentication with NestJS and MongoDB
This project demonstrates how to implement session-based authentication in a NestJS application using MongoDB as the database. It covers user creation, authentication, and route protection.

## Prerequisites
+ Node.js installed on your system.
+ MongoDB installed and running.

## Setup & Installation
1. Install Dependencies: Run `npm install` to install dependencies.
2. Set Up MongoDB Database.
3. Configure the database connection in `app.module.ts` using the MongooseModule.forRoot() method.
4. Run `npm run start:dev` to start the server.

## Features
+ User Registration: Allows users to sign up with a username and password.
+ User Authentication: Users can log in with their credentials.
+ Session Management: Utilizes express-session for session management.
+ Route Protection: Protects routes to ensure only authenticated users can access them.

## Usage
+ Sign Up: Send a POST request to /users/signup with a username and password.
+ Log In: Send a POST request to /users/login with the same credentials.
+ Access Protected Route: After logging in, you can access protected routes.

## Note
Session storage is saved by default in 'MemoryStore,' which is not intended for production use. For production environments, consider using a data store like Redis for stability and performance.

## References
- NestJS Documentation
- MongoDB Documentation
- Passport.js Documentation

## License
This project is licensed under the MIT License.