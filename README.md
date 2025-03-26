# Simple To-Do List Web Application

## Features
- Add new tasks
- Delete existing tasks
- Persist tasks using local storage
- Responsive design
- Simple and clean user interface

## Deployment Instructions

### Local Development
1. Clone the repository
2. Open `index.html` directly in a web browser

### Docker Deployment
1. Build the Docker image:
   ```
   docker build -t <your-dockerhub-username>/todo-list-app:latest .
   ```

2. Run the Docker container locally:
   ```
   docker run -p 8080:80 <your-dockerhub-username>/todo-list-app:latest
   ```

3. Push to Docker Hub:
   ```
   docker login
   docker push <your-dockerhub-username>/todo-list-app:latest
   ```

### Crane Cloud Deployment
1. Create a new project in Crane Cloud
2. Deploy using the Docker image `<your-dockerhub-username>/todo-list-app:latest`
3. Expose port 80

## Notes
- The application uses browser's local storage to persist tasks
- No backend storage is implemented in this version
- Suitable for learning and demonstration purposes
