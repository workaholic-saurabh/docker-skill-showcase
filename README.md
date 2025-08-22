# Docker Multi-Service Application (Red Hat UBI8)

This project demonstrates my **Docker, Docker Compose, and container orchestration** skills by deploying **two independent Apache-based services** running on **Red Hat UBI8 images**.

---

## **Project Overview**
- **Multi-container setup** using Docker Compose.
- **Enterprise-ready base image (Red Hat UBI8)**.
- **Custom static web content** served by Apache HTTP server.
- **Port Mapping:**
  - `web` → [http://localhost:8080](http://localhost:8080)
  - `app` → [http://localhost:8081](http://localhost:8081)

---

## **Technical Highlights**
- **Docker**: Built custom container images using Dockerfiles.
- **Docker Compose**: Orchestrated multiple containers for seamless deployment.
- **Security**: Used UBI8 as a hardened base image.
- **Portability**: Works across environments with minimal configuration.
- **Scalability Ready**: Can be extended to add more services or integrate with Kubernetes.

---

## **Repository Structure**

docker-skill-showcase/
│-- project1/
│ ├── Dockerfile # Builds Apache server (web)
│ └── src/index.html # Web content for Service 1
│
│-- project2/
│ ├── Dockerfile # Builds Apache server (app)
│ └── src/index.html # Web content for Service 2
│
│-- docker-compose.yml # Orchestrates both services

yaml
Copy
Edit

---

## **Setup & Run**
1. **Clone Repository**
```bash
git clone git@github.com:workaholic-saurabh/docker-skill-showcase.git
cd docker-skill-showcase


#Build & Start Containers
docker-compose up -d --build

#Verify Running Containers
docker ps

#Access Applications

Web: http://localhost:8080

App: http://localhost:8081

#Stop Containers.
docker-compose down

#Future Enhancements
Integrate CI/CD pipeline using GitHub Actions/Jenkins.

Deploy to Kubernetes/OpenShift for production scalability.

Add monitoring with Prometheus & Grafana.



Author
Saurabh Chaudhary
https://github.com/workaholic-saurabh
https://www.linkedin.com/in/saurabh-chaudhary-320381361/


