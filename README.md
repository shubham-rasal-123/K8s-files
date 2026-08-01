# Kubernetes Configuration Files

![Kubernetes](https://img.shields.io/badge/Kubernetes-v1.30+-326CE5?style=for-the-badge&logo=kubernetes)
![YAML](https://img.shields.io/badge/YAML-Configuration-CC2927?style=for-the-badge&logo=yaml)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)

A collection of **Kubernetes manifest files** for deploying and managing containerized applications. This repository demonstrates core Kubernetes resources commonly used in real-world deployments and is suitable for learning, testing, and DevOps practice.

---

## 📖 Overview

The **k8s-files** repository contains Kubernetes YAML manifests for deploying workloads, exposing services, and managing application scalability.

It includes the essential Kubernetes resources required to understand application deployment in a Kubernetes cluster.

---

## ✨ Features

- ✅ Kubernetes Pod Configuration
- ✅ ReplicaSet Configuration
- ✅ Deployment Configuration
- ✅ NodePort Service
- ✅ ClusterIP Service
- ✅ YAML-Based Infrastructure
- ✅ Easy Deployment
- ✅ Beginner Friendly
- ✅ DevOps Learning Repository

---

## 📂 Repository Structure

```text
k8s-files/
│
├── pod.yml              # Pod configuration
├── replicaset.yml       # ReplicaSet configuration
├── deployment.yml       # Deployment configuration
├── nodeport.yml         # NodePort Service
├── cluster.yml          # ClusterIP Service
└── README.md            # Documentation
```

---

## 📋 Requirements

| Tool | Version |
|------|---------|

| Kubernetes | v1.30+ |
| kubectl | Latest |
| Docker | Latest |

---

## 🚀 Getting Started

Clone the repository:

```bash
git clone https://github.com/your-github-username/k8s-files.git
```

Navigate to the project directory:

```bash
cd k8s-files
```

Verify cluster connectivity:

```bash
kubectl cluster-info
```

Check cluster nodes:

```bash
kubectl get nodes
```

---

## 📦 Kubernetes Resources

| File | Resource | Purpose |
|------|----------|---------|

| `pod.yml` | Pod | Creates a single containerized application |
| `replicaset.yml` | ReplicaSet | Maintains the desired number of Pod replicas |
| `deployment.yml` | Deployment | Manages rolling updates and ReplicaSets |
| `nodeport.yml` | NodePort Service | Exposes the application externally |
| `cluster.yml` | ClusterIP Service | Exposes the application internally within the cluster |

---

## 🚀 Deployment

### Create a Pod

```bash
kubectl apply -f pod.yml
```

---

### Create a ReplicaSet

```bash
kubectl apply -f replicaset.yml
```

---

### Create a Deployment

```bash
kubectl apply -f deployment.yml
```

---

### Create a ClusterIP Service

```bash
kubectl apply -f cluster.yml
```

---

### Create a NodePort Service

```bash
kubectl apply -f nodeport.yml
```

---

## 🔍 Verification Commands

View Pods:

```bash
kubectl get pods
```

View Deployments:

```bash
kubectl get deployments
```

View ReplicaSets:

```bash
kubectl get rs
```

View Services:

```bash
kubectl get svc
```

View All Resources:

```bash
kubectl get all
```

---

## 📁 File Description

| File | Description |
|------|-------------|

| **pod.yml** | Defines a single Pod resource |
| **replicaset.yml** | Ensures a specified number of Pod replicas |
| **deployment.yml** | Manages application deployment and updates |
| **nodeport.yml** | Creates a NodePort Service for external access |
| **cluster.yml** | Creates a ClusterIP Service for internal communication |

---

## 🌐 Kubernetes Architecture

```text
                 User Request
                      │
                      ▼
               NodePort Service
                      │
                      ▼
              ClusterIP Service
                      │
                      ▼
                Deployment
                      │
                      ▼
                 ReplicaSet
                      │
                      ▼
                     Pods
```

---

## 📚 Useful Commands

Initialize resources:

```bash
kubectl apply -f .
```

Delete all resources:

```bash
kubectl delete -f .
```

Describe a Pod:

```bash
kubectl describe pod <pod-name>
```

View logs:

```bash
kubectl logs <pod-name>
```

Scale a Deployment:

```bash
kubectl scale deployment <deployment-name> --replicas=3
```

Delete a Deployment:

```bash
kubectl delete deployment <deployment-name>
```

---

## 🔒 Best Practices

- Keep YAML files modular and reusable.
- Use Deployments instead of standalone Pods for production.
- Apply labels consistently.
- Use Services for application communication.
- Validate manifests before deployment.
- Store Kubernetes manifests in version control.
- Follow Kubernetes naming conventions.

---

## 🛠️ Technologies Used

- Kubernetes
- kubectl
- Docker
- YAML
- Git
- GitHub

---

## 🤝 Contributing

Contributions are welcome!

To contribute:

- Fork this repository
- Create a feature branch
- Make your changes
- Commit your changes
- Submit a Pull Request

---

## 📄 License

This project is licensed under the **MIT License**.

---

## 👨‍💻 Author

- **Shubham Rasal**

- AWS Certified Solutions Architect – Associate
- DevOps Engineer
- Cloud & Infrastructure Automation Enthusiast

🔗 GitHub:  

**GitHub:** [@shubham-rasal-123](https://github.com/shubham-rasal-123)

---

## ⭐ Support

If you found this repository helpful, consider giving it a **⭐ Star** on GitHub.
