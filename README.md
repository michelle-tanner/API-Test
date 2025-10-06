# Start Using APIs 
Instructions to start using API calls with Postman and data stored in MondoDB Compass. Following these instructions will help you understand how databases (data) are connected to APIs (API Layer).

## Download 
[Node.JS](https://nodejs.org/en/download)

[Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

[Postman](https://www.postman.com/downloads/)
*API Platform designed to simplify the lifecycle of an API. It provides a user-friendly interface for building, testing, documenting, and collaborating on APIs*

[MongoDB](https://www.mongodb.com/?msockid=24c7ed80bfbe616b3404fbbdbec0602c)
*Open-source NoSQL database. Unlike MySQL where you store data in tables with rigid schemas, MongoDB uses a document-oriented data model*

[MongoDB Compass](https://www.mongodb.com/products/tools/compass?msockid=24c7ed80bfbe616b3404fbbdbec0602c)
*MongoDB Compass is a GUI tool for MongoDB. Makes interacting with the database more visual and intuitive*

## Overview
### userController.js 
This is an API controller. It contains the logic for handling HTTP requests that are related to creating the User object/model. It imports the userModel.js file to use for creating JSON files to add to the database. It contains functions that are separate API calls and does a task when called through a URL.
### UserModel.js 
Mongoose schema definition for the MongoDB database to use. It is the blueprint for objects being created and then stored in the MongoDB collection.
### userRoutes.js
This file is an API router and used to define the endpoints (URLs) for your API and link them to the correct functions that handle the logic. Like a traffic controller. When a request comes in, this file looks at the URL and the type of request(e.g. POST or GET) and directs it to the appropriate function in your API controller file.

## Instructions 
1. npm install
2. npm start : make sure you are connected and 'Server is running on port 8000'
3. Go to .env file and paste MONGO_URL into MongoDB Compass
4. In MongoDB Compass, connect to the Database
5. In Postman, Create new Collection > Blank Collection
6. Locate 3 dots on Collection folder > Add request
7. Use GET and POST with the URL to the API call 'fetch' or 'create' and test
