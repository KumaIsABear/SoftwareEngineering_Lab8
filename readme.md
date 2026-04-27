# School App Projects

---

## Lab 8: ASP.NET Core Development

### Exercise 1: Razor Pages Application
* **Description:** ASP.NET Core Razor Pages project using Code First approach.
* **Instructions:** Open in Visual Studio, press F5 to run.

### Exercise 2: MVC Application
* **Description:** ASP.NET Core MVC project using Code First approach.
* **Instructions:** Open in Visual Studio, press F5 to run.

---

## Lab 10: Dockerization & CI/CD Pipeline

### Exercise 1 & 2: Dockerizing ASP.NET Core MVC
* **Description:** Packaged the SchoolAppCoreMVC application into a lightweight Docker Image.
* **Key Files:** `Dockerfile`, `.dockerignore`.
* **Local Image Name:** `myaspnetcoreapp`

### Exercise 3: Ubuntu Server Deployment
* **Description:** Successfully deployed the containerized application to an Ubuntu server (WSL2 environment).
* **Key Steps:**
    * Exported image as `.tar` file and loaded it into the Linux environment.
    * Managed port mapping (**8081:80**) to resolve local port conflicts.
    * Integrated **Docker Compose** for automated container orchestration.

### Exercise 4: CI/CD with GitHub Actions
* **Description:** Implemented a full CI/CD pipeline to automate the build and deployment process.
* **Workflow:**
    1. **Trigger:** Code push to the `master` branch.
    2. **Process:** GitHub Actions (Ubuntu runner) builds the Docker image.
    3. **Registry:** Automatically pushes the verified image to **Docker Hub**.
* **Docker Hub Repository:** `kumadabear/myaspnetcoreapp`

### 🚀 Quick Start (Run from Docker Hub)
Instead of manual building, you can pull and run the latest version directly:

```bash
# Pull the latest image
docker pull kumadabear/myaspnetcoreapp:latest

# Run the container
docker run -d -p 8081:80 --name school-app-container kumadabear/myaspnetcoreapp:latest
