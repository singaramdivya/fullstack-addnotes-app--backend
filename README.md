Notes App Backend
This backend application provides a simple API for managing notes (to-dos). The backend is built with Node.js, Express.js, and MongoDB using Mongoose for data modeling.

Features:

Fetch all notes
Add a new note
Update an existing note
Delete a note

Prerequisites:

Node.js
MongoDB
npm (Node Package Manager)

Installation:
  Clone the repository:
    git clone https://github.com/your-username/notes-app-backend.git
    cd notes-app-backend
  Install the dependencies:
    npm install
  Create a .env file in the root directory and add your MongoDB connection URL:
    MONGODB_URL=your-mongodb-connection-string
    PORT=5000
    
Start the server:
  npm start
  
API Endpoints:
  Get All Notes:
    URL: /
    Method: GET
    Description: Fetch all notes from the database.
    
  Add a New Note:
    URL: /save
    Method: POST
    Description: Add a new note to the database.
    Request Body:
    {
      "text": "Your note text"
    }
    
  Update a Note:
    URL: /update
    Method: POST
    Description: Update an existing note in the database.
    Request Body:
    {
      "_id": "note-id",
      "text": "Updated note text"
    }
Delete a Note:
    URL: /delete
    Method: POST
    Description: Delete a note from the database.
    Request Body:
    {
      "_id": "note-id"
    }

