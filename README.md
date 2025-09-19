# 🐳 DevOps Tools in Docker Containers

This repository provides **pre-configured Docker Compose setups** for popular DevOps tools:  
- Jenkins  
- SonarQube  
- Nexus  
- Tomcat  

Each tool runs in its own isolated container with persistent storage using Docker volumes.  
This setup is designed for **college labs, training, and local testing** – making installation much easier and consistent across machines.

---

## 📦 Prerequisites

Before running these containers, make sure you have:

1. **Docker** installed  
   👉 [Download Docker Desktop](https://www.docker.com/products/docker-desktop/)  
   - On Windows → Install Docker Desktop and enable **WSL2** during setup  
   - On Linux → Install Docker Engine using your package manager  
   - On Mac → Install Docker Desktop  

2. **Docker Compose**  
   - Already included in Docker Desktop  
   - On Linux, install manually:
     ```bash
     sudo apt update
     sudo apt install docker-compose -y
     ```

3. **Check your installation**  
   ```bash
   docker --version
   docker-compose --version

### 1. Clone the Repository
```bash
git clone https://github.com/MaheshMarathe05/Containers.git
cd Containers
### 2.Run Jenkins
```bash
cd jenkins
docker-compose up -d

Access Jenkins → http://localhost:8082

**Get the initial admin password:**

```bash
docker exec jenkins cat /var/jenkins_home/secrets/initialAdminPassword
