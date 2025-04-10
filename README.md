# Note-Taking App

A simple and efficient note-taking application built with a Node.js backend, React frontend, and MongoDB as the database. This app allows users to create, read, update, and delete notes. It’s designed to be easy to use, fast, and deployable with Docker and Docker Compose for containerization.

## Features

- Create, read, update, and delete notes
- Store notes in MongoDB
- User-friendly UI built with React
- RESTful API with Node.js and Express
- Dockerized for easy deployment

## Technologies Used

- **Frontend**: React.js
- **Backend**: Node.js, Express
- **Database**: MongoDB
- **Containerization**: Docker, Docker Compose
- **Version Control**: GitHub

## Installation

Follow these steps to get your development environment set up:

1. Clone this repository:
   ```bash
   git clone https://github.com/confyUK/Note-Taking-App.git
   cd Note-Taking-App
2.Make sure Docker and Docker Compose are installed on your machine. If not, install Docker from the official site.

3. Build and run the Docker containers:
     docker-compose up --build
4. Open your browser and go to http://localhost:80 to view the frontend of the application.
    The backend API is available on http://localhost:5000
   Usage
Frontend
The frontend is built with React and can be accessed via http://localhost:80.

Users can create new notes, view existing notes, update them, and delete them.

Backend
* The backend API is built with Node.js and Express.

* Endpoints include:

   * GET /api/notes: Fetch all notes

   * POST /api/notes: Create a new note

   * PUT /api/notes/:id: Update an existing note

   * DELETE /api/notes/:id: Delete a note

The backend connects to a MongoDB instance to persist the notes.

Docker
This application is containerized using Docker and Docker Compose. The docker-compose.yml file defines three services:

* frontend: React application serving the user interface.

* backend: Node.js application providing the API.

* mongo: MongoDB database for storing the notes.

You can easily build and run the entire application with:
  docker-compose up --build

 Contributing
Feel free to fork this repository and submit issues or pull requests. If you have any suggestions or improvements, please create an issue or submit a pull request.

 Contact
Created by confyUK. Feel free to contact me via GitHub for any questions or suggestions!






