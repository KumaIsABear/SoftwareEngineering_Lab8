# School App Projects
## Exercise 1: Razor Pages Application
[cite_start]Description: ASP.NET Core Razor Pages project using Code First approach. [cite: 1030]
[cite_start]Instructions: Open in Visual Studio, press F5 to run. [cite: 1031]

## Exercise 2: MVC Application
[cite_start]Description: ASP.NET Core MVC project using Code First approach. [cite: 1032]
[cite_start]Instructions: Open in Visual Studio, press F5 to run. [cite: 1033]s

Lab 10: Dockerization & CI/CD Pipeline
Exercise 1 & 2: Dockerizing ASP.NET Core MVC
Description: Packaged the SchoolAppCoreMVC application into a lightweight Docker Image.

Key Files: Dockerfile, .dockerignore.

Image Name: myaspnetcoreapp

Exercise 3: Ubuntu Server Deployment
Description: Successfully deployed the containerized application to an Ubuntu server (WSL2 environment).

Features:

Manual image transfer via .tar files.

Port mapping (8081:80) and environment variable configuration.

Automated orchestration using Docker Compose.

Exercise 4: CI/CD with GitHub Actions
Description: Implemented a full CI/CD pipeline to automate the build and deploy process.

Workflow: 1.  Code is pushed to the master branch.
2.  GitHub Actions triggers a build job using ubuntu-latest.
3.  Docker image is built and automatically pushed to Docker Hub.

Docker Hub Repository: kumadabear/myaspnetcoreapp
