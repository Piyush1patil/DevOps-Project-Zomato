# 🚀 **DevOps Project: ZOMATO Clone App Deployment**
The core objective of this project is to automate the entire software delivery process using a modern DevOps toolchain. When a developer pushes code to the GitHub repository, a series of automated actions are triggered:

CI/CD Pipeline Execution: A Jenkins pipeline automatically checks out the code.

Code Analysis & Security Scanning: The code is analyzed for quality by SonarQube and scanned for vulnerabilities using OWASP Dependency-Check, Trivy, and Docker Scout.

Containerization: A Docker image of the application is built and pushed to Docker Hub.

Deployment: The application is deployed in two ways:

As a Docker container on a primary EC2 instance.

Declaratively to an Amazon EKS (Kubernetes) cluster using ArgoCD for GitOps.

Monitoring: The entire infrastructure, including the Jenkins server and Kubernetes nodes, is monitored using Prometheus and visualized with Grafana dashboards.

Category	              Tools & Technologies
CI/CD Automation	      Jenkins
Version Control	        Git, GitHub
Code Quality & Security	SonarQube, Trivy, OWASP Dependency-Check, Docker Scout
Containerization	      Docker, Docker Hub
Cloud & Infrastructure	AWS (EC2, EKS, IAM, Security Groups)
IaC (Infrastructure as Code)	eksctl
Orchestration & GitOps	  Kubernetes (Amazon EKS), ArgoCD
Monitoring & Visualization	Prometheus, Grafana, Node Exporter
Application Stack	Node.js (as per npm install in the pipeline)
