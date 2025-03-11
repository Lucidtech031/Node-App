# 🚀 DevOps Project: CI/CD Pipeline for Node.js App with Docker & Kubernetes  

## 📌 Project Overview  
This project demonstrates a **CI/CD pipeline** for a **Node.js application** using:  
✅ **GitHub Actions** for automation  
✅ **Docker** for containerization  
✅ **Docker Hub** for image storage  
✅ **Kubernetes (EKS)** for deployment  

The pipeline automates **building, testing, containerizing, and deploying** the app to a Kubernetes cluster.

---

## 🛠️ Tech Stack  
- **Node.js** – Backend application  
- **Docker** – Containerization  
- **GitHub Actions** – CI/CD automation  
- **AWS EKS (Elastic Kubernetes Service)** – Kubernetes hosting  
- **kubectl** – Kubernetes command-line tool  

---

## 📂 Project Structure  
📁 project-root/
│– 📂 src/                # Node.js application files
│– 📄 Dockerfile          # Docker image configuration
│– 📄 .github/workflows/  # GitHub Actions pipeline
│– 📄 deployment.yaml     # Kubernetes deployment
│– 📄 service.yaml        # Kubernetes service
│– 📄 README.md           # Project documentation

---

## 🚀 Getting Started  

### **1️⃣ Clone the Repository**  
```bash
git clone https://github.com/lucidtech031/node-app.git
cd node-app
```
Set Up Environment Variables
Create a .env file in the project root with:
PORT=3000
```bash
docker build -t node-app .
docker run -p 3000:3000 node-app
```
🏗️ CI/CD Pipeline Workflow

🛠️ GitHub Actions Pipeline
	1.	Push to GitHub → Triggers workflow
	2.	Build & Test → Runs unit tests
	3.	Docker Build → Creates an image
	4.	Push to Docker Hub → Stores the image
	5.	Deploy to Kubernetes → Applies kubectl commands

 Apply Kubernetes Configuration
 ```bash
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```
Check Deployment
```bash
kubectl get pods
kubectl get services
```
🔗 CI/CD Pipeline Status

👨‍💻 Contributors
.Marcos Batista Macias

📜 License
This project is MIT Licensed
---

### **How to Customize This for Your Repo**
1. Replace **"your-username"** with your **GitHub username**.  
2. Replace **"your-repo"** with your **repository name**.  
3. Update the **project description, technologies, and setup steps** if needed.  
