# AWS Deployment Assignment

This project is part of my DevOps AWS Deployment assignment.

The objective of this assignment was to deploy a Flask backend and an Express frontend using different AWS deployment methods.

## Tasks Completed

### Task 1 – Single EC2

Deployed the Flask backend and Express frontend on a single Amazon EC2 instance.

### Task 2 – Separate EC2

Deployed the Flask backend and Express frontend on two separate EC2 instances and configured communication between them.

### Task 3 – Docker, ECR and ECS

Dockerized the Flask backend and Express frontend and deployed them on AWS using:

- Docker
- Amazon ECR
- Amazon ECS Fargate
- Amazon VPC
- Security Groups

## Project Structure

```text
AWS-Satyam/
│
├── backend/
│   ├── app.py
│   ├── Dockerfile
│   ├── .dockerignore
│   └── requirements.txt
│
├── frontend/
│   ├── server.js
│   ├── package.json
│   ├── Dockerfile
│   ├── .dockerignore
│   ├── public/
│   │   └── style.css
│   └── views/
│       └── index.ejs
│
├── docker-compose.yml
├── ecs-task-definition.json
├── ecs-task-trust-policy.json
└── README.md

Technologies Used
Python
Flask
Node.js
Express.js
Docker
Docker Compose
AWS EC2
AWS ECR
AWS ECS
AWS VPC
GitHub
Local Docker Setup

To build the Docker images:

docker compose build

To start the containers:
docker compose up -d

To check the running containers:

docker compose ps

To stop the containers:

docker compose down
AWS Deployment

For the final deployment, the Docker images were pushed to Amazon ECR and then deployed using Amazon ECS Fargate.

The ECS cluster used for the deployment was:

docker-satyam-cluster

The ECS service was:

docker-satyam-service

The service was configured with one desired task and one running task.

Live Application

The deployed application can be accessed at:

http://35.154.117.142:3000

The application was tested successfully and the form submission returned   
Submit Successful

## Author

**Satyam Kumar Singh**
