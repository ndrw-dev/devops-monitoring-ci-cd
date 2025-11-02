# 🚀 DevOps Monitoring CI/CD Project

This project demonstrates a complete CI/CD workflow and monitoring setup using Jenkins, Docker, Docker Hub, Prometheus, and Grafana — with a sample Flask web application.

---

## 🧱 Project Overview

The project automates the build, deployment, and monitoring of a simple web app.  
When code is pushed to GitHub:
- Jenkins automatically builds a Docker image.
- The image is pushed to Docker Hub.
- The updated container is redeployed on the server.
- Prometheus and Grafana monitor metrics from both the system and Jenkins.

---

## ⚙️ Main Components

### **Flask App**
A simple Python web app used as the deployment target for CI/CD.

### **Jenkins CI/CD**
Handles continuous integration and deployment:
- Automatically pulls source code from GitHub.
- Builds and pushes Docker images to Docker Hub.
- Deploys the latest version of the app.

### **Prometheus**
Collects and stores metrics from:
- Node Exporter (server metrics)
- Jenkins (build status and metrics)
- Prometheus itself

### **Grafana**
Visualizes data from Prometheus with dashboards for:
- CPU, RAM, and disk usage
- Jenkins build status
- Container uptime and system performance

### **Node Exporter**
Collects hardware and OS-level metrics for Prometheus.

---

## 🧩 Architecture Summary

1. Developer pushes code to GitHub.  
2. Jenkins triggers CI/CD pipeline automatically.  
3. Docker builds and redeploys the Flask container.  
4. Prometheus scrapes metrics from Node Exporter and Jenkins.  
5. Grafana visualizes the collected data in real time.

---

## 📊 Dashboards

Grafana dashboards include:
- **Node Exporter Full**: Full system monitoring 

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|----------|
| **Jenkins** | CI/CD pipeline automation |
| **Docker & Docker Hub** | Containerization and image hosting |
| **Prometheus** | Monitoring and alerting system |
| **Grafana** | Data visualization |
| **Node Exporter** | Server metrics collector |
| **Flask** | Demo web application |

---

## 🧠 Key Learnings

- How to set up Jenkins pipelines for Dockerized applications.  
- Automating deployment using Docker Hub.  
- Integrating Prometheus and Grafana for real-time infrastructure monitoring.  
- Building a full DevOps workflow from development → deployment → monitoring.

---

## 👨‍💻 Author

**To Ly Tien Dat (Andrew To)**  
📧 [Contact](dattovl17@gmail.com)  
🐙 [GitHub: ndrw-dev](https://github.com/ndrw-dev)

---

## 🏁 Result

A fully automated DevOps workflow:
- Code changes → automatically built and deployed.
- Metrics → continuously monitored with alerts and dashboards.
- All services run inside a local Linux VM.

![View Stage - Jenkins Pipeline](https://media.discordapp.net/attachments/1331318634294808711/1434454952968716388/JenkinsPipeline_ViewStage.png?ex=690863c7&is=69071247&hm=7b4ba4d2f7b96d8a0f6c04b6925ca4840ad11431d6fc35f19348e6784b1db81c&=&format=webp&quality=lossless&width=1557&height=728)

![Result on Grafana](https://media.discordapp.net/attachments/1331318634294808711/1434454949546295376/ResultOnGrafana.png?ex=690863c6&is=69071246&hm=220812065083fd9f8b3878fe5af50d4dad31a77674010625b1d5d0e856a77cba&=&format=webp&quality=lossless&width=1557&height=776)

