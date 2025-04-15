
## Overview

This document explains the Continuous Integration and Continuous Deployment (CI/CD) pipeline built for the GPI 2025 DevOps (Basic Level) project.

---

##  Trigger

The pipeline is triggered on every `push` to the `main` branch.

---

## ⚙️ Workflow: `.github/workflows/nodejs.yml`

### Steps:

1. **Checkout code** from GitHub
2. **Set up Node.js** environment
3. **Install dependencies** using `npm install`
4. **Build Docker image** with the `Dockerfile`
5. **Login to DockerHub** using GitHub Secrets
6. **Tag and push image** to DockerHub

---

##  Secrets Used

- `DOCKER_USERNAME`: DockerHub username
- `DOCKER_PASSWORD`: DockerHub password

---

##  DockerHub Output

After a successful pipeline run, the image is pushed to:

