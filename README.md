
📌 Project Title

Pwani Cloud Run Flask API

📖 Project Description

This project is a containerized Python Flask API deployed on Google Cloud Run.
It demonstrates how to build, containerize, and deploy a serverless web application using Docker and Google Cloud Platform services.

The application exposes REST API endpoints and runs in a fully managed serverless environment.

🚀 Features
Flask REST API
Docker containerization
Cloud Run serverless deployment
Public internet access
JSON API responses
Runtime metadata endpoint

🌐 API Endpoints
/

Returns a welcome message.

{
  "message": "Welcome to Cloud Run",
  "Name": "Annet Gatende"
}
/health

Used to check if the service is running.

{
  "status": "healthy"
}
/info

Returns runtime information from the container.

{
  "hostname": "container-id",
  "timestamp": "current-time"
}

🐳 Run Locally with Docker
1. Build Docker image
docker build -t pwani-cloudrun-app .
2. Run container
docker run -p 8080:8080 pwani-cloudrun-app
3. Access app
http://localhost:8080/
http://localhost:8080/health
http://localhost:8080/info

☁️ Deploy to Google Cloud Run
gcloud run deploy pwani-cloudrun-app \
  --source . \
  --allow-unauthenticated \
  --region europe-west1

🔗 Live Deployment URL
https://pwani-cloudrun-app-776357600646.europe-west1.run.app

🛠 Tech Stack
Python (Flask)
Docker
Google Cloud Run
Google Cloud Build
Git & GitHub

👩‍💻 Author
Annet Gatende