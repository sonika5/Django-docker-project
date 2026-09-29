# 🐳 Django Web Application with Docker

A Django web application containerized using **Docker** and deployed on an **AWS EC2** instance.

## 📌 Project Overview

This project demonstrates how a Django web application can be packaged into a Docker image and run inside a Docker container.

The application is built with Django and configured to run on port `8000`. Docker provides a consistent environment for running the application, while AWS EC2 is used to host the container.

## 🛠️ Technologies Used

- 🐍 Python
- 🎯 Django
- 🐳 Docker
- ☁️ AWS EC2
- 🐧 Ubuntu Linux
- 🔧 Git & GitHub

## 📂 Project Structure

```text
python-web-app/
│
├── Dockerfile
├── requirements.txt
├── README.md
│
└── devops/
    ├── manage.py
    ├── demo/
    └── devops/
```

## 🐳 Dockerfile

The Dockerfile uses **Ubuntu** as the base image and:

- Sets `/app` as the working directory
- Copies the required project files
- Installs Python, pip, and virtual environment support
- Creates a Python virtual environment
- Installs the required Python dependencies
- Exposes port `8000`
- Starts the Django development server on `0.0.0.0:8000`

## 🚀 Running the Project

The application can be run using Docker with the following steps:

- Clone the GitHub repository
- Build the Docker image using the Dockerfile
- Run the Docker container with port `8000` mapped to the host
- Access the Django application through port `8000`

## ☁️ AWS EC2 Deployment

The Dockerized Django application was deployed on an **AWS EC2 Ubuntu instance**.

- Built the Docker image on the EC2 instance
- Ran the Django application inside a Docker container
- Mapped EC2 port `8000` to container port `8000`
- Configured the EC2 security group to allow inbound traffic on port `8000`
- Accessed the application through the EC2 public IP and port `8000`

## 🎯 What I Learned

Through this project, I practiced:

- 🐳 Creating and working with Dockerfiles
- 📦 Building Docker images
- 🚀 Running Docker containers
- 🔌 Mapping container ports to host ports
- 🐧 Working with Ubuntu Linux
- ☁️ Deploying a containerized application on AWS EC2
- 🔧 Using Git and GitHub for version control

