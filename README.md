# Assignment Pipeline

A simple Node.js and Express application containerized using Docker and designed to demonstrate basic CI/CD and deployment workflow practices.

## Overview

This project was created as part of an assignment to demonstrate:

* Node.js application development
* Express.js server setup
* Docker containerization
* Dependency management using npm
* Basic deployment readiness
* CI/CD workflow integration

The application exposes a simple HTTP endpoint and can be run locally or inside a Docker container.

---

## Tech Stack

### Backend

* Node.js
* Express.js

### DevOps

* Docker
* GitHub
* GitHub Actions

---

## Project Structure

```bash
assignment-pipeline/
│
├── index.js
├── package.json
├── package-lock.json
├── Dockerfile
├── .gitignore
└── README.md
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/shivamani90141-byte/assignment-pipeline.git
```

Move into the project directory:

```bash
cd assignment-pipeline
```

Install dependencies:

```bash
npm install
```

---

## Running Locally

Start the application:

```bash
npm start
```

The server will run on:

```bash
http://localhost:3000
```

Expected response:

```text
Hello World! My automated pipeline is successful.
```

---

## API Endpoint

| Method | Endpoint | Description                        |
| ------ | -------- | ---------------------------------- |
| GET    | /        | Returns application status message |

---

## Docker Setup

Build Docker image:

```bash
docker build -t assignment-pipeline .
```

Run Docker container:

```bash
docker run -p 3000:3000 assignment-pipeline
```

Access application:

```bash
http://localhost:3000
```

---

## CI/CD

The repository includes a GitHub Actions workflow that can be used to automate build and deployment processes whenever code changes are pushed to the repository.

Typical CI/CD stages include:

* Source code checkout
* Dependency installation
* Application build
* Docker image creation
* Container registry publishing
* Deployment automation

---

## Future Improvements

* Environment variable configuration
* Multiple API endpoints
* Request validation
* Structured logging
* Health check endpoints
* Unit testing
* Cloud deployment
* Monitoring and observability

---

## Author

**Shivamani**

GitHub:
https://github.com/shivamani90141-byte

---

## License

This project is licensed under the MIT License.
