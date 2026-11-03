# Kubernetes Namespace Task

## 📌 Project Overview

This project demonstrates the setup of a local Kubernetes cluster using Minikube and the creation and management of Kubernetes namespaces.

The objective is to understand Kubernetes cluster basics and namespace management using `kubectl`.

## 🛠️ Technologies Used

- Docker
- Minikube
- Kubernetes
- kubectl
- Windows 11
- WSL 2
- Visual Studio Code

## 🏗️ Project Architecture

```text
Windows 11
    |
    ├── WSL 2
    |
    ├── Docker Desktop
    |
    └── Minikube
          |
          └── Kubernetes Cluster
                |
                ├── default
                ├── kube-system
                ├── kube-public
                ├── kube-node-lease
                └── dev-namespace
```

## 🚀 Steps Performed

### 1. Start Minikube

Started the local Kubernetes cluster using Docker as the driver.

```bash
minikube start --driver=docker
```

### 2. Verify Kubernetes Cluster

Checked the cluster information.

```bash
kubectl cluster-info
```

### 3. Verify Kubernetes Nodes

```bash
kubectl get nodes
```

### 4. View Existing Namespaces

```bash
kubectl get namespaces
```

### 5. Create a New Namespace

Created a custom namespace named `dev-namespace`.

```bash
kubectl create namespace dev-namespace
```

### 6. Verify Namespace

```bash
kubectl get namespaces
```

### 7. Describe Namespace

```bash
kubectl describe namespace dev-namespace
```

### 8. Delete Namespace

```bash
kubectl delete namespace dev-namespace
```

## 📸 Screenshots

All screenshots are available inside the screenshots folder.


## 📂 Project Structure

```text
Kubernetes-Task/
│
├── README.md
├── commands.txt
│
└── screenshots/
    ├── minikube-start.png
    ├── kubectl-get-nodes.png
    ├── kubectl-get-namespaces.png
    ├── namespace-create.png
    ├── namespace-verify.png
    ├── namespace-describe.png
    └── namespace-delete.png
```


## 🎯 Learning Outcomes

- Understanding Kubernetes cluster setup.
- Learning Minikube and kubectl.
- Creating and managing Kubernetes namespaces.
- Understanding namespace isolation and resource organization.

---

**Author:** Sethu Raman

**Project:** Kubernetes Namespace Task
