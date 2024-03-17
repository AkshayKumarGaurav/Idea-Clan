# Express GraphQL Server with User and Post Functionalities

This project comprises a Node.js application that utilizes Express and Apollo Server for implementing a GraphQL API. It encompasses functionalities for user registration and login, seamlessly integrated with MongoDB database.


## Deployed-Link
[link](https://idea-clan-xzi6.onrender.com/)


## Functionalities
### User Authentication
- **User Registration** : Users can register with a email, name, username, and password.

- **Login User** : Registered users can log in using their email and password.

### Post Management
- **Create Post (Authenticated)** : Authenticated users can create posts. Only logged-in users can create posts, and posts are associated with the user who created them.

- **Get User Posts (Authenticated)** : Authenticated users can retrieve their own posts. Only posts belonging to the logged-in user are returned.


## Project Structure
- src/
  - configs/
    - db.js: MongoDB connection configuration.
  - GraphQL/
    - user.typeDefs.js: GraphQL type definitions for user operations.
    - user.resolvers.js: Resolvers for user operations.
    - posts.typeDefs.js: GraphQL type definitions for post operations.
    - posts.resolvers.js: Resolvers for post operations.
  - models/
    - user.model.js: Mongoose model for User schema.
    - post.model.js: Mongoose model for Post schema.
  - index.js: Entry point for the server.


## Setup

1. **Clone the repository** 
```bash
  https://github.com/AkshayKumarGaurav/Idea-Clan.git
```
2. **Install dependencies**
```bash
  cd server
  npm install
```

3. **Set up environment variables** 
Create a .env file with the following variables:
```bash
PORT = 8080

SECRET_KEY = your_secret_key

MONGODB_URL = your_mongodb_uri
```
4. **Start the server**
```bash
npm start
Access the server at :- http://localhost:8080/
```




## Technologies Used

- Express.js: Web application framework for Node.js.
- Apollo Server Express: GraphQL server for Express.js.
- Mongoose: MongoDB object modeling for Node.js.
- bcryptjs: Library for hashing passwords.
- jsonwebtoken: Implementation of JSON Web Tokens.
