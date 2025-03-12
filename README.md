# Todo Application

A full-stack todo application built with React, Node.js, and MongoDB, using Docker for containerization.

## Tech Stack

- **Frontend**: React
- **Backend**: Node.js
- **Database**: MongoDB
- **Containerization**: Docker

## Prerequisites

Before you begin, ensure you have installed:
- [Docker](https://www.docker.com/get-started)

## Getting Started

1. Clone the repository:
```bash
git clone <https://github.com/aleedurrani/MLOPS-Activity-03>
```

2. Start the application:
```bash
docker-compose up
```

This will start three containers:
- Client (React) - running on `http://localhost:3000`
- Server (Node.js) - running on `http://localhost:5000`
- MongoDB - running on `localhost:27017`

To stop the application:
```bash
docker-compose down
```

## Project Structure

├── client/ # React frontend
├── server/ # Node.js backend
└── docker-compose.yml


## Development

The application uses Docker volumes for hot-reloading:
- Frontend changes will automatically refresh in the browser
- Backend changes will automatically restart the server
- MongoDB data persists between container restarts