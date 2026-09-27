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
├── 🐳 Dockerfile
├── 📦 requirements.txt
├── 📄 README.md
│
└── 📁 devops/
    ├── manage.py
    ├── 📁 demo/
    └── 📁 devops/

## 🐳 Dockerfile

The Dockerfile uses **Ubuntu** as the base image and:

- Sets `/app` as the working directory
- Copies the required project files
- Installs Python, pip, and virtual environment support
- Creates a Python virtual environment
- Installs the required Python packages
- Exposes port `8000`
- Starts the Django development server on `0.0.0.0:8000`

## 🚀 Running the Project
1️⃣ Clone the Repository
git clone https://github.com/sonika5/Django-docker-project.git
cd Django-docker-project
2️⃣ Build the Docker Image
docker build -t django-web-app .
3️⃣ Run the Docker Container
docker run -it -p 8000:8000 django-web-app

The application will be available at:

http://localhost:8000/

##☁️ AWS EC2 Deployment

The Docker container was also run on an AWS EC2 Ubuntu instance.

Port 8000 was mapped from the EC2 host to the Docker container:

EC2 Port 8000
      ↓
Docker Port 8000
      ↓
Django Application

The EC2 security group was configured to allow inbound traffic on port 8000.

🎯 What I Learned

Through this project, I practiced:

🐳 Creating a Dockerfile
📦 Building Docker images
🚀 Running Docker containers
🔌 Mapping container ports to host ports
🐧 Working with Ubuntu on AWS EC2
☁️ Deploying a containerized application on AWS
🔧 Managing source code with Git and GitHub
