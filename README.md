Node.js API with Express.js for MongoDB CRUD Operations
Overview
This project provides a simple Node.js API using Express.js to perform basic CRUD operations on a MongoDB server. The API supports the following methods: GET, POST, UPDATE, and DELETE. The data model includes fields for firstname, lastname, country, gender, phonenumber, and email.

Prerequisites
Before running the application, make sure you have the following installed:

Node.js
npm (Node Package Manager)
MongoDB
Setup
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/node-express-mongodb-api.git
Install dependencies:

bash
Copy code
cd node-express-mongodb-api
npm install
Configure MongoDB connection:

Update the MongoDB connection string in the config.js file.

Usage
Run the Server
bash
Copy code
npm start
The API server will run on http://localhost:5000.

Endpoints
1. Get All Users
Method: GET
Endpoint: /api/users
2. Get User by ID
Method: GET
Endpoint: /api/users/:id
3. Create a New User
Method: POST
Endpoint: /api/users
Request Body:
json
Copy code
{
  "firstName": "John",
  "lastName": "Doe",
  "country": "USA",
  "gender": "Male",
  "phoneNumber": "1234567890",
  "email": "john.doe@example.com"
}
4. Update User by ID
Method: PUT
Endpoint: /api/users/:id
Request Body:
json
Copy code
{
  "country": "Egypt",
  "phonenumber": "011254623548"
}
5. Delete User by ID
Method: DELETE
Endpoint: /api/users/:id
Contributing
Feel free to contribute to the project by opening issues or submitting pull requests.

License
This project is licensed under the MIT License - see the LICENSE file for details.