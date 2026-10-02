# Docker Web Project

A simple static web application running inside an Nginx Docker container.

## Technologies

- Docker
- Nginx
- Git
- GitHub
- HTML

## Project Structure

docker-web-project/
├── index.html
├── Dockerfile
├── README.md
└── .gitignore

## How to Build

docker build -t docker-web-project:v1 .

## How to Run

docker run -d \
  --name docker-web-container \
  -p 8084:80 \
  docker-web-project:v1

## Test

curl http://localhost:8084

## Architecture

Browser
   ↓
Host Port 8084
   ↓
Docker Container
   ↓
Nginx Port 80
   ↓
index.html
