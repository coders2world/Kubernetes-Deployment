# Task 9: Docker Basics – Containerizing an Application

## Overview
Containerizing a simple Python Flask application using Docker.

## Tools Used
- Docker
- Python 3.11
- Flask

## Project Structure
my-docker-app/
├── app.py
├── requirements.txt
└── Dockerfile

## Commands Used

# Build image
docker build -t my-flask-app:1.0 .

# Run container
docker run -d -p 5000:5000 --name flask-container my-flask-app:1.0

# Check running containers
docker ps

# View logs
docker logs flask-container

# Stop and cleanup
docker stop flask-container
docker rm flask-container
docker rmi my-flask-app:1.0

## Steps Performed
1. Installed Docker and verified installation
2. Created a simple Python Flask application
3. Wrote a Dockerfile
4. Built Docker image using docker build
5. Ran container using docker run on port 5000
6. Inspected containers and logs
7. Stopped and removed containers and images

## Deliverables
- Dockerfile
- Running container screenshot