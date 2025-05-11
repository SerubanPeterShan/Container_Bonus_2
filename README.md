# Todo List Web Application

A simple, responsive Todo List web application containerized using Docker and Podman.

## Features

- Add new tasks
- Mark tasks as complete/incomplete
- Delete tasks
- Persistent storage using localStorage
- Responsive design
- Containerized deployment

## Prerequisites

- Docker
- Podman

## Running with Docker

1. Build the Docker image:
```bash
docker build -t todo-app .
```

2. Run the container:
```bash
docker run -d -p 8080:80 todo-app
```

3. Access the application at `http://localhost:8080`

## Running with Podman

1. Build the Podman image:
```bash
podman build -t todo-app -f Containerfile .
```

2. Run the container:
```bash
podman run -d -p 8080:80 localhost/todo-app
```

3. Access the application at `http://localhost:8080`

## Screenshots

Screenshots of the application and containerization process can be found in the `screenshots` directory, organized by platform.

## Project Structure

```
.
├── index.html          # Main HTML file
├── styles.css          # CSS styles
├── script.js           # JavaScript functionality
├── Dockerfile         # Docker configuration
├── Containerfile      # Podman configuration
└── screenshots/       # Screenshots directory
    ├── docker/        # Docker screenshots
    └── podman/        # Podman screenshots
``` 